---

copyright:
  years: 2017, 2021
lastupdated: "2021-11-05"

keywords: terraform quickstart, terraform getting started, terraform tutorial

subcollection: ibm-cloud-provider-for-terraform

---

{{site.data.keyword.attribute-definition-list}}


# Getting started with Terraform on {{site.data.keyword.cloud_notm}}
{: #getting-started}

Terraform on {{site.data.keyword.cloud_notm}} enables predictable and consistent provisioning of {{site.data.keyword.cloud_notm}} platform, classic infrastructure, and VPC infrastructure resources so that you can rapidly build complex, multi-tier cloud environments, and enable Infrastructure as Code (IaC). 
{: shortdesc}

Looking for a managed Terraform on {{site.data.keyword.cloud_notm}} solution? Try out [{{site.data.keyword.bplong_notm}}](/docs/schematics?topic=schematics-getting-started). With {{site.data.keyword.bpshort}}, you can use the Terraform scripting language that you are familiar with, but you don't have to worry about setting up and maintaining the Terraform command line and the {{site.data.keyword.cloud_notm}} Provider plug-in. {{site.data.keyword.bpshort}} also provides pre-defined Terraform templates that you can easily install from the {{site.data.keyword.cloud_notm}} catalog.
{: tip}




## Step 1: Installing the Terraform CLI
{: #tf_installation}

Use these steps to install the Terraform CLI. 
{: shortdesc}

1. Create a `terraform` folder on your local machine, and navigate to your `terraform` folder. 
    ```
    mkdir terraform && cd terraform
    ```
    {: pre}

2. Download the [Terraform version](https://releases.hashicorp.com/terraform){: external} that you want. The {{site.data.keyword.cloud_notm}} Provider plug-in for Terraform currently supports Terraform version 0.12.x, 0.13.x, 0.14.x, 0.15.x, and 1.0 only. Make sure to select a supported Terraform version. 
3. Extract the Terraform `zip` file and copy the files to your `terraform` directory. 
4. Set the environment `PATH` variable to your Terraform files.
    ```
    export PATH=$PATH:$HOME/terraform
    ```
    {: pre}

5. Verify that the installation is successful by using a `terraform` command.
    ```
    terraform
    ```
    {: pre}

    Example output:
    ```
    Usage: terraform [-version] [-help] <command> [args]

    The available commands for execution are listed below.
    The most common, useful commands are shown first, followed by
    less common or more advanced commands. If you're just getting
    started with Terraform, stick with the common commands. For the
    other commands, please read the help and docs before usage.

    Common commands:
    apply              Builds or changes infrastructure
    console            Interactive console for Terraform interpolations
    destroy            Destroy Terraform-managed infrastructure
    env                Workspace management
    fmt                Rewrites config files to canonical format
    get                Download and install modules for the configuration
    graph              Create a visual graph of Terraform resources
    import             Import existing infrastructure into Terraform
    init               Initialize a Terraform working directory
    login              Obtain and save credentials for a remote host
    logout             Remove locally-stored credentials for a remote host
    output             Read an output from a state file
    plan               Generate and show an execution plan
    providers          Prints a tree of the providers used in the configuration
    refresh            Update local state file against real resources
    show               Inspect Terraform state or plan
    taint              Manually mark a resource for recreation
    untaint            Manually unmark a resource as tainted
    validate           Validates the Terraform files
    version            Prints the Terraform version
    workspace          Workspace management

    All other commands:
    0.12upgrade        Rewrites pre-0.12 module source code for v0.12
    debug              Debug output management (experimental)
    force-unlock       Manually unlock the terraform state
    push               Obsolete command for Terraform Enterprise legacy (v1)
    state              Advanced state management

    ```
    {: screen}

## Step 2: Configuring the {{site.data.keyword.cloud_notm}} Provider plug-in
{: #install_provider}

After the Terraform CLI installation is complete, you must set up and configure the {{site.data.keyword.cloud_notm}} Provider plug-in for Terraform so that you can start working with resources and services in {{site.data.keyword.cloud_notm}}. 
{: shortdesc}

The following steps show how to set up the provider plug-in for Terraform v0.13.x or higher. If you installed or want to use an earlier version of Terraform, install the provider plug-in by following the steps in [Terraform v0.12.x and earlier](/docs/ibm-cloud-provider-for-terraform?topic=ibm-cloud-provider-for-terraform-setup_cli#install-provider-v12). 
{: note}

1. In your Terraform installation directory, create a folder for your first Terraform on {{site.data.keyword.cloud_notm}} project and navigate into the folder. This folder is used to store all configuration files and variable definitions. 
    ```
    mkdir myproject && cd myproject
    ```
    {: pre}

2. Create a `versions.tf` file with the following content. In this file, specify the {{site.data.keyword.cloud_notm}} Provider plug-in version that you want to use with the `version` parameter. If no version is specified, Terraform on {{site.data.keyword.cloud_notm}} automatically uses the latest version. For a list of supported versions, see the [{{site.data.keyword.cloud_notm}} Provider plug-in releases](https://github.com/IBM-Cloud/terraform-provider-ibm/releases){: external}.

    ```
    terraform {
        required_providers {
            ibm = {
            source = "IBM-Cloud/ibm"
            version = "<provider_version>"       
            }
        }
    }
    ```
    {: codeblock}

    The version is specified in the following format `<MAJOR_VERSION>.<MINOR_VERSION>.<PATCH>`. You can modify the version constraint operator in this example by using one of the [supported operators in Terraform](https://www.terraform.io/docs/language/expressions/version-constraints.html#version-constraint-syntax){: external}. 
    {: tip}

3. [Create or retrieve an {{site.data.keyword.cloud_notm}} API key](/docs/account?topic=account-userapikey#create_user_key). The API key is used to authenticate with the {{site.data.keyword.cloud_notm}} platform and to determine your permissions for {{site.data.keyword.cloud_notm}} services.
4. Create a variables file that is named `terraform.tfvars` and specify the {{site.data.keyword.cloud_notm}} API key that you retrieved. In addition, you specify the region where you want your {{site.data.keyword.cloud_notm}} resources to be created. If no region is specified, Terraform on {{site.data.keyword.cloud_notm}} automatically creates your resources in the `us-south` region. Variables that are defined in the `terraform.tfvars` file are automatically loaded by Terraform when the {{site.data.keyword.cloud_notm}} Provider plug-in is initialized and you can reference them in every Terraform configuration file that you use. 

    Because the `terraform.tfvars` file contains confidential information, do not push this file to a version control system. This file is meant to be on your local system only. 
    {: important}

    ```
    ibmcloud_api_key = "<ibmcloud_api_key>"
    region = "<region>"
    ```
    {: codeblock}

5. Create a provider configuration file that is named `provider.tf`. Use this file to configure the {{site.data.keyword.cloud_notm}} Provider plug-in with the {{site.data.keyword.cloud_notm}} API key from your `terraform.tfvars` file. The plug-in uses this key to access {{site.data.keyword.cloud_notm}} and to work with your {{site.data.keyword.cloud_notm}} service. To access a variable value from the `terraform.tfvars` file, you must first declare the variable in the `provider.tf` file and then reference the variable by using the `var.<variable_name>` syntax . 

    ```
    variable "ibmcloud_api_key" {}
    variable "region" {}

    provider "ibm" {
        ibmcloud_api_key   = var.ibmcloud_api_key
        region = var.region
        }
    ```
    {: codeblock}

    **Classic infrastructure, Functions, Power Systems**: Additional parameters are required when configuring the {{site.data.keyword.cloud_notm}} Provider plug-in. To find sample configurations for these services, see [Specifying the `provider` block](/docs/ibm-cloud-provider-for-terraform?topic=ibm-cloud-provider-for-terraform-provider-reference#provider-example). 
    {: tip}

## Step 3: Testing your configuration

Now that you configured the {{site.data.keyword.cloud_notm}} Provider plug-in for your resource you can start using Terraform on {{site.data.keyword.cloud_notm}} to initialize, execute plan and apply commands to provision the resource. For more information, about Terraform commands to test your configuration, see [Provisioning IBM Cloud resources](/docs/ibm-cloud-provider-for-terraform?topic=ibm-cloud-provider-for-terraform-manage_resources#provision_resources).
{: shortdesc}

For an overview of the Terraform resources and data sources that you can use, see the [{{site.data.keyword.cloud_notm}} Provider plug-in documentation](https://registry.terraform.io/providers/IBM-Cloud/ibm/latest/docs){: external}. 





