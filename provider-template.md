---

copyright:
  years: 2017, 2021
lastupdated: "2021-09-14"

keywords: terraform templates, templates, sample terraform templates, private catalog

subcollection: ibm-cloud-provider-for-terraform

---

{:DomainName: data-hd-keyref="APPDomain"}
{:DomainName: data-hd-keyref="DomainName"}
{:android: data-hd-operatingsystem="android"}
{:api: .ph data-hd-interface='api'}
{:apikey: data-credential-placeholder='apikey'}
{:app_key: data-hd-keyref="app_key"}
{:app_name: data-hd-keyref="app_name"}
{:app_secret: data-hd-keyref="app_secret"}
{:app_url: data-hd-keyref="app_url"}
{:audio: .audio}
{:authenticated-content: .authenticated-content}
{:beta: .beta}
{:c#: .ph data-hd-programlang='c#'}
{:c#: data-hd-programlang="c#"}
{:cli: .ph data-hd-interface='cli'}
{:codeblock: .codeblock}
{:curl: #curl .ph data-hd-programlang='curl'}
{:curl: .ph data-hd-programlang='curl'}
{:deprecated: .deprecated}
{:dotnet-standard: .ph data-hd-programlang='dotnet-standard'}
{:download: .download}
{:external: .external target="_blank"}
{:external: target="_blank" .external}
{:faq: data-hd-content-type='faq'}
{:fuzzybunny: .ph data-hd-programlang='fuzzybunny'}
{:generic: data-hd-operatingsystem="generic"}
{:generic: data-hd-programlang="generic"}
{:gif: data-image-type='gif'}
{:go: .ph data-hd-programlang='go'}
{:help: data-hd-content-type='help'}
{:hide-dashboard: .hide-dashboard}
{:hide-in-docs: .hide-in-docs}
{:important: .important}
{:ios: data-hd-operatingsystem="ios"}
{:java: #java .ph data-hd-programlang='java'}
{:java: .ph data-hd-programlang='java'}
{:java: data-hd-programlang="java"}
{:javascript: .ph data-hd-programlang='javascript'}
{:javascript: data-hd-programlang="javascript"}
{:middle: .ph data-hd-position='middle'}
{:navgroup: .navgroup}
{:new_window: target="_blank"}
{:node: .ph data-hd-programlang='node'}
{:note: .note}
{:objectc: .ph data-hd-programlang='Objective C'}
{:objectc: data-hd-programlang="objectc"}
{:org_name: data-hd-keyref="org_name"}
{:php: .ph data-hd-programlang='PHP'}
{:php: data-hd-programlang="php"}
{:pre: .pre}
{:preview: .preview}
{:python: .ph data-hd-programlang='python'}
{:python: data-hd-programlang="python"}
{:release-note: data-hd-content-type='release-note'}
{:right: .ph data-hd-position='right'}
{:route: data-hd-keyref="route"}
{:row-headers: .row-headers}
{:ruby: .ph data-hd-programlang='ruby'}
{:ruby: data-hd-programlang="ruby"}
{:runtime: architecture="runtime"}
{:runtimeIcon: .runtimeIcon}
{:runtimeIconList: .runtimeIconList}
{:runtimeLink: .runtimeLink}
{:runtimeTitle: .runtimeTitle}
{:screen: .screen}
{:script: data-hd-video='script'}
{:service: architecture="service"}
{:service_instance_name: data-hd-keyref="service_instance_name"}
{:service_name: data-hd-keyref="service_name"}
{:shortdesc: .shortdesc}
{:space_name: data-hd-keyref="space_name"}
{:step: data-tutorial-type='step'}
{:step: data-tutorial-type='step'} 
{:subsection: outputclass="subsection"}
{:support: data-reuse='support'}
{:swift: #swift .ph data-hd-programlang='swift'}
{:swift: .ph data-hd-programlang='swift'}
{:swift: data-hd-programlang="swift"}
{:table: .aria-labeledby="caption"}
{:term: .term}
{:terraform: .ph data-hd-interface='terraform'}
{:tip: .tip}
{:tooling-url: data-tooling-url-placeholder='tooling-url'}
{:topicgroup: .topicgroup}
{:troubleshoot: data-hd-content-type='troubleshoot'}
{:tsCauses: .tsCauses}
{:tsResolve: .tsResolve}
{:tsSymptoms: .tsSymptoms}
{:tutorial: data-hd-content-type='tutorial'}
{:ui: .ph data-hd-interface='ui'}
{:unity: .ph data-hd-programlang='unity'}
{:url: data-credential-placeholder='url'}
{:user_ID: data-hd-keyref="user_ID"}
{:vbnet: .ph data-hd-programlang='vb.net'}
{:video: .video}


# Sample Terraform templates for {{site.data.keyword.cloud_notm}}
{: #provider-template}

Explore the sample {{site.data.keyword.cloud}} Terraform templates, onboard the templates to your private catalogs, and try your templates by using {{site.data.keyword.bpshort}} workspace.

Deploy [Sample templates](#sample-templates) by using IBM Cloud service. <br>
Browse [Code snippets](#code-snippets) by IBM Cloud service.

## Onboard to IBM Cloud private catalog
{: #provider-onboard}

Click the **Onboard to IBM Cloud catalog** button to automatically load the following sample Terraform templates into your catalog. In order to run this automation, press the **Create** button in **Create an action** page in the console.
{: shortdesc}

For more information, about how the Ansible based automation is configured to load the template to private catalogs? refer to [Onboard to IBM Catalog readme file](https://github.com/Cloud-Schematics/onboard-to-ibm-catalog/blob/main/README.md).
{: note}

<img src="images/onboardtoibmcatalog.png" usemap="#image-map2"><map name="image-map2"><area target="_blank" alt="bulk onboard Terraform templates into private catalog" title="onboard Terraform template to private catalog" href="https://cloud.ibm.com/schematics/actions/create?name=demo-catalogs&url=https://github.com/Cloud-Schematics/onboard-to-ibm-catalog" coords="1,1,200,40" shape="rect"></map>

## Sample templates
{: #sample-templates}

Following are the lsit of sample templates that allows you to provision resource by using {{site.data.keyword.bpshort}} workspace. 

- [Kubernetes and OpenShift](#kubnernetes-openshift)
- [VPC infrastructure](#vpc-templates)
- [Observability](observability-templates)
- [Storage](#storage-templates)
- [Classic infrastructure service](#classic-infra-templates)
- [Account management and IAM](#account-mgt-iam)


## Code snippets
{: #code-snippets}

The code snippets provides the templates that you can use to understand how to configure IBM Cloud service. You can also use the snippets as a starting point for your custom templates.
{: shortdesc}

- [API Gateway](#api-gwy-snippet)
- [Certificate Manager](#cert-mgr-snippet)
- [Cloud Databases templates](#cloud-db-snippet)
- [Cloud Foundry](#cloud-foundry-snippet)
- [Direct Link](#dl-snippet)
- [DNS templates](#dns-snippet)
- [Event Streams](#event-stream-snippet)
- [Functions](#func-snippet)
- [Identity & Access (IAM)](#iam-snippet)
- [Internet templates ](#internet-snippet)
- [Key Management Service](#kms-snippet)
- [Kubernetes templates](#kubernetes-snippet)
- [Object Storage templates](#cos-snippet)
- [Power Systems templates](#power-sys-snippet)
- [Resource Management templates](#resource-mgt-snippet)
- [Schematics templates](#schematics-snippet)
- [Transit Gateway templates](#transit-gwy-snippet)
- [VPC infrastructure templates (Gen 2 compute)](#vpc-gen2-snippet)


## Templates
{: #sample}

### Kubernetes and OpenShift
{: #kubnernetes-openshift}

In the **Workspace details** page, click **Next** button to view the **Create** button active to create {{site.data.keyword.bpshort}} workspace.
{: note}

|  Template | Description | Provision |
| ---- | ---- | --- |
| [Kubernetes cluster on VPC](https://github.com/Cloud-Schematics/multizone-iks-on-vpc-cluster) | Provision of a Kubernetes cluster on an existing VPC network, with private application load balancers.| <img usemap="#deploybutton_mapcs10" alt="Auto deployment button"  src="images/autodeploy_button.png"><map name="deploybutton_mapcs10" alt="This image leads to create a workspace."><area alt="Deploy to IBM Cloud" title="Deploy to IBM Cloud" href="https://cloud.ibm.com/schematics/workspaces/create?repository=https://github.com/Cloud-Schematics/multizone-iks-on-vpc-cluster&terraform_version=terraform_v0.12" target="_blank" coords="1,3,139,20"  shape="rect"></map>|
| [{{site.data.keyword.openshiftshort}} cluster on classic infrastructure](https://github.com/Cloud-Schematics/openshift-cluster) | Provision of a simple Red Hat OpenShift cluster on Classic infrastructure. | <img usemap="#deploybutton_mapcs11" alt="Auto deployment button"  src="images/autodeploy_button.png"><map name="deploybutton_mapcs11" alt="This image leads to create a workspace."><area alt="Deploy to IBM Cloud" title="Deploy to IBM Cloud" href="https://cloud.ibm.com/schematics/workspaces/create?repository=https://github.com/Cloud-Schematics/openshift-cluster&terraform_version=terraform_v0.13" target="_blank" coords="1,3,139,20"  shape="rect"></map>|
| [{{site.data.keyword.openshiftshort}} cluster on Classic infrastrucutre for development environment](https://github.com/Cloud-Schematics/openshift-dev-cluster) | Provision of a Red Hat Openshift cluster on Classic infrastructure for a development team with IBM Cloud Operation, Red Hat CodeReady.| <img usemap="#deploybutton_mapcs11" alt="Auto deployment button"  src="images/autodeploy_button.png"><map name="deploybutton_mapcs11" alt="This image leads to create a workspace."><area alt="Deploy to IBM Cloud" title="Deploy to IBM Cloud" href="https://cloud.ibm.com/schematics/workspaces/create?repository=https://github.com/Cloud-Schematics/openshift-dev-cluster&terraform_version=terraform_v0.13" target="_blank" coords="1,3,139,20"  shape="rect"></map>|
| [Microservices with ingress on Kubernetes cluster](https://github.com/Cloud-Schematics/iks-on-vpc-deploy-demo-ingress-app) | Deploy a sample app with ingress on your existing Kubernetes cluster on VPC.| <img usemap="#deploybutton_mapcs4" alt="Auto deployment button"  src="images/autodeploy_button.png"><map name="deploybutton_mapcs4" alt="This image leads to create a workspace."><area alt="Deploy to IBM Cloud" title="Deploy to IBM Cloud" href="https://cloud.ibm.com/schematics/workspaces/create?repository=https://github.com/Cloud-Schematics/iks-on-vpc-deploy-demo-ingress-app&terraform_version=terraform_v0.13" target="_blank" coords="1,3,139,20"  shape="rect"></map>|
| [Microservices with load balancer on Kubernetes cluster](https://github.com/Cloud-Schematics/iks-on-vpc-deploy-demo-load-balancer-app) | Deploy a sample app with load balance on your existing Kubernetes cluster on VPC.| <img usemap="#deploybutton_mapcs5" alt="Auto deployment button"  src="images/autodeploy_button.png"><map name="deploybutton_mapcs5" alt="This image leads to create a workspace."><area alt="Deploy to IBM Cloud" title="Deploy to IBM Cloud" href="https://cloud.ibm.com/schematics/workspaces/create?repository=https://github.com/Cloud-Schematics/iks-on-vpc-deploy-demo-load-balancer-app&terraform_version=terraform_v0.13" target="_blank" coords="1,3,139,20"  shape="rect"></map>|
{: caption="Kubernetes and OpenShift Terraform templates to provision resource using {{site.data.keyword.bpshort}} workspace" caption-side="top"}


### VPC infrastructure
{: #vpc-templates}

|  Template | Description | Provision |
| ---- | ---- | --- |
| [Multiple VSIs on VPC with block storage volume and a load balancer](https://github.com/Cloud-Schematics/vpc-vsi-with-volumes-and-lb) | Provision multiple virtual servers each with a block storage volume on VPC, across a number of subnets, and connected with a single load balancer. | <img usemap="#deploybutton_mapcs14" alt="Auto deployment button"  src="images/autodeploy_button.png"><map name="deploybutton_mapcs14" alt="This image leads to create a workspace."><area alt="Deploy to IBM Cloud" title="Deploy to IBM Cloud" href="https://cloud.ibm.com/schematics/workspaces/create?repository=https://github.com/Cloud-Schematics/vpc-vsi-with-volumes-and-lb&terraform_version=terraform_v0.12" target="_blank" coords="1,3,139,20"  shape="rect"></map>|
| [Multi-tier VPC with bastion and VSIs](https://github.com/Cloud-Schematics/multitier-bastion-vpc-lamp) | Provision multi-tier infrastructure with VPC, SSH, Bastion host, front-end, and backend servers.| <img usemap="#deploybutton_mapcs8" alt="Auto deployment button"  src="images/autodeploy_button.png"><map name="deploybutton_mapcs8" alt="This image leads to create a workspace."><area alt="Deploy to IBM Cloud" title="Deploy to IBM Cloud" href="https://cloud.ibm.com/schematics/workspaces/create?repository=https://github.com/Cloud-Schematics/multitier-bastion-vpc-lamp&terraform_version=terraform_v0.12" target="_blank" coords="1,3,139,20"  shape="rect"></map>|
| [Multi-tier VPC network](https://github.com/Cloud-Schematics/multitier-vpc-network) | Provision of a multi-tier infrastructure with VPC, in a single region up to 3 zones, ACL and public gateways.| <img usemap="#deploybutton_mapcs9" alt="Auto deployment button"  src="images/autodeploy_button.png"><map name="deploybutton_mapcs9" alt="This image leads to create a workspace."><area alt="Deploy to IBM Cloud" title="Deploy to IBM Cloud" href="https://cloud.ibm.com/schematics/workspaces/create?repository=https://github.com/Cloud-Schematics/multitier-vpc-network&terraform_version=terraform_v0.12" target="_blank" coords="1,3,139,20"  shape="rect"></map>|
{: caption="VPC Terraform templates to provision resource using {{site.data.keyword.bpshort}} workspace" caption-side="top"}


### Observability
{: #observability-templates}

|  Template | Description | Provision |
| ---- | ---- | --- |
| [Observability service instance](https://github.com/Cloud-Schematics/terraform-ibm-observability) | Provision an instance of all the Observability services on IBM Cloud such as IBM Cloud Log Analysis, IBM Cloud Monitoring, and IBM Cloud Activity Tracker in your account.| <img usemap="#deploybutton_mapcs13" alt="Auto deployment button"  src="images/autodeploy_button.png"><map name="deploybutton_mapcs13" alt="This image leads to create a workspace."><area alt="Deploy to IBM Cloud" title="Deploy to IBM Cloud" href="https://cloud.ibm.com/schematics/workspaces/create?repository=https://github.com/Cloud-Schematics/terraform-ibm-observability&terraform_version=terraform_v0.13" target="_blank" coords="1,3,139,20"  shape="rect"></map>|
| [Observability agents for Kubernetes cluster](https://github.com/Cloud-Schematics/iks-logging-and-monitoring) | Deploy logging and monitoring agents onto your existing {{site.data.keyword.containerlong_notm}} cluster on VPC. | <img usemap="#deploybutton_mapcs3" alt="Auto deployment button"  src="images/autodeploy_button.png"><map name="deploybutton_mapcs3" alt="This image leads to create a workspace."><area alt="Deploy to IBM Cloud" title="Deploy to IBM Cloud" href="https://cloud.ibm.com/schematics/workspaces/create?repository=https://github.com/Cloud-Schematics/iks-logging-and-monitoring&terraform_version=terraform_v0.13" target="_blank" coords="1,3,139,20"  shape="rect"></map>|
| [Configure integrations for Log Analysis service](https://github.com/Cloud-Schematics/logdna-provider-example) | Configure the Log Analysis service instance in IBM Cloud to integrate with `Slack`, `PagerDuty` and `Webhooks`. | <img usemap="#deploybutton_mapcs7" alt="Auto deployment button"  src="images/autodeploy_button.png"><map name="deploybutton_mapcs7" alt="This image leads to create a workspace."><area alt="Deploy to IBM Cloud" title="Deploy to IBM Cloud" href="https://cloud.ibm.com/schematics/workspaces/create?repository=https://github.com/Cloud-Schematics/logdna-provider-example&terraform_version=terraform_v0.13" target="_blank" coords="1,3,139,20"  shape="rect"></map>|
| [Configure alerts and dashboard for Monitoring services](https://github.com/Cloud-Schematics/sysdig-provider-example) | Configure the monitoring service instance in IBM Cloud with alerts and dashboard. | <img usemap="#deploybutton_mapcs12" alt="Auto deployment button"  src="images/autodeploy_button.png"><map name="deploybutton_mapcs12" alt="This image leads to create a workspace."><area alt="Deploy to IBM Cloud" title="Deploy to IBM Cloud" href="https://cloud.ibm.com/schematics/workspaces/create?repository=https://github.com/Cloud-Schematics/sysdig-provider-example&terraform_version=terraform_v0.12" target="_blank" coords="1,3,139,20"  shape="rect"></map>|
{: caption="Observability Terraform templates to provision resource using {{site.data.keyword.bpshort}} workspace" caption-side="top"}


### Storage
{: #storage-templates}

|  Template | Description | Provision |
| ---- | ---- | --- |
| [IBM Cloud Object Storage bucket with encryption](https://github.com/Cloud-Schematics/kms-encrypted-cos-bucket) | Provision IBM Cloud Object Storage with IBM Key Protect integration. | <img usemap="#deploybutton_mapcs6" alt="Auto deployment button"  src="images/autodeploy_button.png"><map name="deploybutton_mapcs6" alt="This image leads to create a workspace."><area alt="Deploy to IBM Cloud" title="Deploy to IBM Cloud" href="https://cloud.ibm.com/schematics/workspaces/create?repository=https://github.com/Cloud-Schematics/kms-encrypted-cos-bucket&terraform_version=terraform_v0.13" target="_blank" coords="1,3,139,20"  shape="rect"></map>|
{: caption="Storage Terraform templates to provision resource using {{site.data.keyword.bpshort}} workspace" caption-side="top"}


### Account management and IAM
{: #account-mgt-iam}

|  Template | Description | Provision |
| ---- | ---- | --- |
| [Clone users to new account](https://github.com/Cloud-Schematics/add-all-users-to-new-account)| Clone all the IAM users from one IBM Cloud account into another IBM Cloud account. | <img usemap="#deploybutton_mapcs1" alt="Auto deployment button"  src="images/autodeploy_button.png"><map name="deploybutton_mapcs1" alt="This image leads to create a workspace."><area alt="Deploy to IBM Cloud" title="Deploy to IBM Cloud" href="https://cloud.ibm.com/schematics/workspaces/create?repository=https://github.com/Cloud-Schematics/add-all-users-to-new-account&terraform_version=terraform_v0.13" target="_blank" coords="1,3,139,20"  shape="rect"></map>|
{: caption="Account management and IAM Terraform templates to provision resource using {{site.data.keyword.bpshort}} workspace" caption-side="top"}

### Classic infrastructure service
{: #classic-infra-templates}

|  Template | Description | Provision |
| ---- | ---- | --- |
| [Autoscale the Classic VSIs](https://github.com/Cloud-Schematics/classic-vsi-autoscaling-solution) | Autoscale the classic VSIs using {{site.data.keyword.bpshort}}, {{site.data.keyword.openwhisk_short}}, and Sysdig. | <img usemap="#deploybutton_mapcs2" alt="Auto deployment button"  src="images/autodeploy_button.png"><map name="deploybutton_mapcs2" alt="This image leads to create a workspace."><area alt="Deploy to IBM Cloud" title="Deploy to IBM Cloud" href="https://cloud.ibm.com/schematics/workspaces/create?repository=https://github.com/Cloud-Schematics/classic-vsi-autoscaling-solution&terraform_version=terraform_v0.13" target="_blank" coords="1,3,139,20"  shape="rect"></map>|
{: caption="Classic infrastructure templates to provision resource using {{site.data.keyword.bpshort}} workspace" caption-side="top"}


## Snippets
{: #tf_snippet}

### API Gateway templates
{: #api-gwy-snippet}

| Name | Description and resources | Code |
| --- | --- | --- |
| `ibm-api-gateway` | Create an <a href="/docs/api-gateway?topic=api-gateway-whatis_apigw">IBM Cloud API Gateway</a> service instance to set up an API for an IBM Cloud service of your choice. You can specify the API endpoint that you want to use to access your service, and define subscription keys so that developers can securely consume your API. <br><br> **Resources** <ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px">**ibm_resource_instance**</li><li style="margin:0px; padding:0px">**ibm_api_gateway_endpoint**</li><li style="margin:0px; padding:0px">**ibm_api_gateway**</li><li style="margin:0px; padding:0px">**ibm_api_gateway_endpoint_subscription**</li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-api-gateway)|


## Certificate Manager templates
{: #cert-mgr-snippet}

| Name | Description and resources | Code |
| --- | --- | --- |
| `ibm-certificate-manager-order` | Create an {{site.data.keyword.cis_full_notm}} instance with a domain, and use <a href="/docs/certificate-manager?topic=certificate-manager-about-certificate-manager">IBM Cloud Certificate Manager</a> to generate a TLS certificate for this domain.<br><br>**Resources**<br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px">**ibm_resource_instance**</li><li style="margin:0px; padding:0px">**ibm_cis**</li><li style="margin:0px; padding:0px">**ibm_cis_domain**</li><li style="margin:0px; padding:0px">**ibm_certificate_manager_order**</li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-certificate-manager/ibm-certificate-manager-order)|

## Cloud Foundry templates
{: #cloud-foundry-snippet}

| Name | Description and resources | Code |
| --- | --- | --- |
| `ibm-app` | Create and deploy a Cloud Foundry app in {{site.data.keyword.cloud_notm}}.<br><br>**Resources**<br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px">**null_resource**</li><li style="margin:0px; padding:0px">**ibm_app_route**</li><li style="margin:0px; padding:0px">**ibm_service_instance**</li><li style="margin:0px; padding:0px">**ibm_service_key**</li><li style="margin:0px; padding:0px">**ibm_app**</li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-app)|

## Direct Link templates
{: #dl-snippet}

| Name | Description and resources | Code |
| --- | --- | --- |
| `ibm-dl-gateway` | Create a speed and reliable direct link gateways, virtual connections, offering information, routers, and ports by using the resources.<br><br>**Resources**<br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px">**ibm_dl_gateway**</li><li style="margin:0px; padding:0px">**ibm_dl_virtual_connection**</li><li style="margin:0px; padding:0px">**ibm_is_vpc**</li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-direct-link)|

## Event Streams templates
{: #event-stream-snippet}

| Name | Description and resources | Code |
| --- | --- | --- |
| `ibm-event-streams` | Create a communication through an Event Streams instance, topic instance, or Kafka consumer application to connect an existing event stream instances and its topic instance by using {{site.data.keyword.bplong_notm}} workspace.<br><br>**Resources**<br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px">**ibm_resource_instance**</li><li style="margin:0px; padding:0px">**ibm_event_streams_topic**</li><li style="margin:0px; padding:0px">**kafka_consumer_app**</li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-event-streams)|

## Functions templates
{: #func-snippet}

| Name | Description and resources | Code |
| --- | --- | --- |
| `ibm-function-cloudant-trigger` | Create a Cloudant NoSQL service instance and a Python app deployment that creates the **database demo** database in your service instance. Then, you create an action with {{site.data.keyword.cloud_notm}} functions that is triggered when you add or edit documents to your database.<br><br>**Resources**<br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px">**null_resource**</li><li style="margin:0px; padding:0px">**ibm_service_instance**</li><li style="margin:0px; padding:0px">**ibm_service_key**</li><li style="margin:0px; padding:0px">**ibm_app_route**</li><li style="margin:0px; padding:0px">**ibm_app**</li><li style="margin:0px; padding:0px">**ibm_function_package**</li><li style="margin:0px; padding:0px">**ibm_function_action**</li><li style="margin:0px; padding:0px">**ibm_function_trigger**</li><li style="margin:0px; padding:0px">**ibm_function_rule**</li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-function-cloudant-trigger)|

## Identity & Access (IAM) templates
{: #iam-snippet}

| Name | Description and resources | Code |
| --- | --- | --- |
| `ibm-iam-custom-role` | Create a custom role in IBM Cloud Identity and Access Management (IAM) for IBM Cloud Key Protect.<br><br>**Resources**<br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px">**ibm_iam_custom_role**</li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-iam-custom-role)|
| `ibm-iam-policy` | Create an access policy in IBM Cloud Identity and Access Management (IAM) to grant permissions for a resource group to a user.<br><br>**Resources**<br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px">**ibm_iam_user_policy**</li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-iam-policy)|
| `ibm-iam-policy` | Create an access group in {{site.data.keyword.IBM_notm}} {{site.data.keyword.iamshort}} and assign this access group permission to a resource group. Then, you add users to your access group and assign these users access to IBM Cloud Kubernetes Service, classic IBM Cloud infrastructure, and Cloud Foundry.<br><br><strong>Resources</strong><br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px"><code>ibm_iam_access_group</code></li><li style="margin:0px; padding:0px"><code>ibm_iam_access_group_policy</code></li><li style="margin:0px; padding:0px"><code>ibm_iam_user_invite</code></li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-iam-user-invite)|

## Key Management Service templates
{: #kms-snippet}

| Name | Description and resources | Code |
| --- | --- | --- |
| `ibm-key-management-service` | Create an {{site.data.keyword.cos_full_notm}} service instance with a bucket to store your data and provide a key management service resource for Hyper Protect Crypto Services and Key Protect service instance with a root key. This allow access between these services with an IBM Cloud Identity and Access Management policy.<br><br>**Resources**<br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px">**ibm_kms_key**</li><li style="margin:0px; padding:0px">**ibm_kp_key**</li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-kms)|

## Kubernetes templates
{: #kubernetes-snippet}

| Name | Description and resources | Code |
| --- | --- | --- |
| `vpc-classic-cluster` | Create an {{site.data.keyword.containerfull_notm}} cluster in a Virtual Private Cloud (VPC) for Generation 1 compute with worker nodes in a default worker pool that you spread across two zones. You can provision an IBM Cloud Object Storage service, and bind this service to the cluster.<br><br>**Resources**<br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px">**ibm_is_vpc**</li><li style="margin:0px; padding:0px">**ibm_is_subnet**</li><li style="margin:0px; padding:0px">**ibm_container_vpc_cluster**</li><li style="margin:0px; padding:0px">**ibm_container_vpc_worker_pool**</li><li style="margin:0px; padding:0px">**ibm_resource_instance**</li><li style="margin:0px; padding:0px">**ibm_container_bind_service**</li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-cluster/vpc-classic-cluster)|
| `vpc-Gen2-cluster` | Create an {{site.data.keyword.containerfull_notm}} cluster in a Virtual Private Cloud (VPC) for Generation 2 compute with worker nodes in a default worker pool that you spread across two zones. Also, you provision an IBM Cloud Object Storage service, and bind this service to the cluster.<br><br>**Resources**<br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px">**ibm_is_vpc**</li><li style="margin:0px; padding:0px">**ibm_is_subnet**</li><li style="margin:0px; padding:0px">**ibm_container_vpc_cluster**</li><li style="margin:0px; padding:0px">**ibm_container_vpc_worker_pool**</li><li style="margin:0px; padding:0px">**ibm_resource_instance**</li><li style="margin:0px; padding:0px">**ibm_container_bind_service**</li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-cluster/vpc-gen2-cluster)|
| `ibm-iks-classic-ROKS` | Create a Red Hat View GitHub repository on IBM Cloud cluster that runs version 3.11 of the View GitHub repository Container Platform.<br><br>**Resources**<br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px">**ibm_container_cluster**</li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-iks-classic-ROKS)|
| `ibm-cluster-update` | Cordon and drain your worker nodes to update the IBM Cloud Kubernetes Service cluster master and worker nodes to the latest version.<br><br><strong>Resources</strong><br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px"><code>null_resource</code></li><li style="margin:0px; padding:0px"><code>ibm_container_cluster</code></li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-cluster-update)|
| `cluster-worker-pool-zone` | Create an IBM Cloud Kubernetes Service cluster with a default worker pool that is spread across two zones. Also, you create another worker pool and bind an IBM Cloud service of your choice to the cluster.<br><br><strong>Resources</strong><br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px"><code>ibm_container_cluster</code></li><li style="margin:0px; padding:0px"><code>ibm_container_worker_pool_zone_attachment</code></li><li style="margin:0px; padding:0px"><code>ibm_container_worker_pool</code></li><li style="margin:0px; padding:0px"><code>ibm_service_instance</code></li><li style="margin:0px; padding:0px"><code>ibm_service_key</code></li><li style="margin:0px; padding:0px"><code>ibm_container_bind_service</code></li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-cluster/cluster-worker-pool-zone)|
| `ibm-storage-cos` | Set up Helm in an {{site.data.keyword.containerlong_notm}} cluster to install the {{site.data.keyword.cos_full_notm}} Helm plug-in. Then, you create an {{site.data.keyword.cos_full_notm}} service instance where you can store data from the apps in your cluster. You also learn how to create a Kubernetes persistent volume claim (PVC) to create a bucket in your {{site.data.keyword.cos_full_notm}} instance. Also to deploy an app in the cluster that mounts your {{site.data.keyword.cos_full_notm}} bucket.<br><br><strong>Resources</strong><br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px"><code>ibm_resource_instance</code></li><li style="margin:0px; padding:0px"><code>ibm_container_bind_service</code></li><li style="margin:0px; padding:0px"><code>kubernetes_secret</code></li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-storage-cos)|
| `ibm-openshift-job` | Create and execute a secured shell script in an {{site.data.keyword.openshiftlong_notm}} cluster by using an Terraform on {{site.data.keyword.cloud_notm}} template. This template creates a Kubernetes configmap that includes a reference to a shell script. Then, you create a pod that mounts the configmap as a volume and executes the shell script.<br><br><strong>Resources</strong><br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px"><code>kubernetes_secret</code></li><li style="margin:0px; padding:0px"><code>kubernetes_config_map</code></li><li style="margin:0px; padding:0px"><code>kubernetes_job</code></li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-openshift-job)|
| `portworx` | Set up Helm in an {{site.data.keyword.containerlong_notm}} software-defined storage (SDS) cluster to install Portworx as a storage solution. Make sure that this template requires an SDS cluster on Bare Metal worker nodes. After you installed Portworx, you can create persistent volume claims (PVC) to store data on local storage of your worker nodes. For more information, about Portworx and how to create an SDS cluster, see <a href="/docs/containers?topic=containers-portworx">Storing data on SDS with Portworx</a>.<br><br><strong>Resources</strong><br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px"><code>random_id</code></li><li style="margin:0px; padding:0px"><code>kubernetes_secret</code></li><li style="margin:0px; padding:0px"><code>helm_release</code></li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/portworx)|
| `ibm-lbaas` | Create an {{site.data.keyword.loadbalancer_full}} for a classic virtual server instance. You configure the load balancer to manage incoming HTTPS and HTTP network traffic and set up health monitoring for your virtual server instance.<br><br><strong>Resources</strong><br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px"><code>ibm_compute_ssl_certificate</code></li><li style="margin:0px; padding:0px"><code>ibm_compute_ssh_key</code></li><li style="margin:0px; padding:0px"><code>ibm_compute_vm_instance</code></li><li style="margin:0px; padding:0px"><code>ibm_lbaas</code></li></li><li style="margin:0px; padding:0px"><code>ibm_lbaas_server_instance_attachment</code></li><li style="margin:0px; padding:0px"><code>ibm_lbaas_health_monitor</code></li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-lbaas)|
| `ibm-logdna-cluster-integration` | Create an IBM Cloud cluster integration service to configure IBM Cloud provider such as Helm, Kubernetes. Then, you can use a  resource role binding to fetch resource key, and agents to log through resource role binding.<br><br><strong>Resources</strong><br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px"><code>random_id</code></li><li style="margin:0px; padding:0px"><code>kubernetes_role_binding</code></li><li style="margin:0px; padding:0px"><code>helm_release</code></li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-logdna-cluster-integration)|


## Transit Gateway templates
{: #transit-gwy-snippet}

| Name | Description and resources | Code |
| --- | --- | --- |
| `ibm-transit-gateway` | Create a transit gateways, list available connections, and locations for the gateways.<br><br>**Resources**<br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px">**ibm_tg_gateway**</li><li style="margin:0px; padding:0px">**ibm_tg_connection**</li><li style="margin:0px; padding:0px">**ibm_is_vpc**</li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-transit-gateway)|

## Cloud Databases templates
{: #cloud-db-snippet}

| Name | Description and resources | Code |
| --- | --- | --- |
| `ibm-database` | Create a classic virtual server instance and an {{site.data.keyword.cloud_notm}} database for PostgreSQL instance, and set up connectivity between the instances.<br><br><strong>Resources</strong><br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px"><code>ibm_compute_vm_instance</code></li><li style="margin:0px; padding:0px"><code>ibm_resource_group</code></li><li style="margin:0px; padding:0px"><code>ibm_database</code></li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-database)|

## DNS templates
{: #dns-snippet}

| Name | Description and resources | Code |
| --- | --- | --- |
| `ibm-private-dns` | Create an {{site.data.keyword.vpc_short}} and an {{site.data.keyword.dns_full_notm}} instance, and add the VPC as a permitted network to the DNS service instance. Then, you create different types of DNS records.<br><br><strong>Resources</strong><br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px"><code>ibm_is_vpc</code></li><li style="margin:0px; padding:0px"><code>ibm_resource_instance</code></li><li style="margin:0px; padding:0px"><code>ibm_dns_zone</code></li><li style="margin:0px; padding:0px"><code>ibm_dns_resource_record</code></li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-private-dns)|

## Internet templates 
{: #internet-snippet}

| Name | Description and resources | Code |
| --- | --- | --- |
| `ibm-cis` | Create an IBM Cloud Internet Service instance and configure the instance with health check monitoring, origin pool, global load-balancing, DNS records, firewall, and limit the rate rules.<br><br><strong>Resources</strong><br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px"><code>ibm_cis</code></li><li style="margin:0px; padding:0px"><code>ibm_cis_domain_settings</code></li><li style="margin:0px; padding:0px"><code>ibm_cis_domain</code></li><li style="margin:0px; padding:0px"><code>ibm_cis_edge_functions_action</code></li><li style="margin:0px; padding:0px"><code>ibm_cis_edge_functions_trigger</code></li><li style="margin:0px; padding:0px"><code>ibm_cis_healthcheck</code></li><li style="margin:0px; padding:0px"><code>ibm_cis_origin_pool</code></li><li style="margin:0px; padding:0px"><code>ibm_cis_global_load_balancer</code></li><li style="margin:0px; padding:0px"><code>ibm_cis_dns_record</code></li><li style="margin:0px; padding:0px"><code>ibm_cis_firewall</code></li><li style="margin:0px; padding:0px"><code>ibm_cis_rate_limit</code></li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-cis)|

## Object Storage templates
{: #cos-snippet}

| Name | Description and resources | Code |
| --- | --- | --- |
| `ibm-cos-bucket` | Create an <a href="/docs/cloud-object-storage?topic=cloud-object-storage-about-cloud-object-storage">IBM Cloud Object Storage</a> service instance in IBM Cloud and your first bucket to persistently store data.<br><br><strong>Resources</strong><br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px"><code>ibm_resource_group</code></li><li style="margin:0px; padding:0px"><code>ibm_resource_instance</code></li><li style="margin:0px; padding:0px"><code>ibm_cos_bucket</code></li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-cos-bucket)|

## Power Systems templates
{: #power-sys-snippet}

| Name | Description and resources | Code |
| --- | --- | --- |
| `ibm-power` | Create an {{site.data.keyword.powerSys_notm}} instance with a public and a private network that mounts the system volumes. You can also create an SSH key to access the instance.<br><br><strong>Resources</strong><br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px"><code>ibm_pi_key</code></li><li style="margin:0px; padding:0px"><code>ibm_pi_network</code></li><li style="margin:0px; padding:0px"><code>ibm_pi_volume</code></li><li style="margin:0px; padding:0px"><code>ibm_pi_instance</code></li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-power)|

## Resource Management templates
{: #resource-mgt-snippet}

| Name | Description and resources | Code |
| --- | --- | --- |
| `ibm-resource-instance` | Create an {{site.data.keyword.cos_full_notm}} service instance with HMAC credentials, and configure custom timeouts for creating, updating, or deleting the instance.<br><br><strong>Resources</strong><br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px"><code>ibm-resource-instance</code></li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-resource-instance)|

## Schematics templates
{: #schematics-snippet}

| Name | Description and resources | Code |
| --- | --- | --- |
| `ibm-schematics` | Retrieve the Terraform on {{site.data.keyword.cloud_notm}} state file and output variables for a {{site.data.keyword.bpshort}} workspace by using a {{site.data.keyword.bpshort}} data source. For more information, about how to use the data source, see <a href="/docs/schematics?topic=schematics-remote-state">Managing cross-workspace state access with Terraform on {{site.data.keyword.cloud_notm}}</a>.<br><br><strong>Resources</strong><br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px"><code>N/A</code></li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-schematics)|

## VPC infrastructure templates (Gen 2 compute)
{: #vpc-gen2-snippet}

| Name | Description and resources | Code |
| --- | --- | --- |
| `ibm-is-ng` | Create a Virtual Private Cloud (VPC) for Generation 2 compute, configure a VPC load balancer with custom routing rules. Then, add a virtual server instance to your VPC that you can access from the internet by using a public IP address. Then, create another VPC Gen 2 and configure it with a VPN gateway with custom IPSec and IKE networking rules. You also learn how to create VPC Gen 2 block storage volumes.<br><br><strong>Resources</strong><br><ul style="margin:0px 0px 0px 20px; padding:0px"><li style="margin:0px; padding:0px"><code>ibm_is_vpc</code></li><li style="margin:0px; padding:0px"><code>ibm_is_vpc_route</code></li><li style="margin:0px; padding:0px"><code>ibm_is_subnet</code></li><li style="margin:0px; padding:0px"><code>ibm_is_lb</code></li><li style="margin:0px; padding:0px"><code>ibm_is_lb_listener</code></li><li style="margin:0px; padding:0px"><code>ibm_is_lb_listener_policy</code></li><li style="margin:0px; padding:0px"><code>ibm_is_lb_listener_policy_rule</code></li><li style="margin:0px; padding:0px"><code>ibm_is_vpn_gateway</code></li><li style="margin:0px; padding:0px"><code>ibm_is_vpn_gateway_connection</code></li><li style="margin:0px; padding:0px"><code>ibm_is_ssh_key</code></li><li style="margin:0px; padding:0px"><code>ibm_is_instance</code></li><li style="margin:0px; padding:0px"><code>ibm_is_floating_ip</code></li><li style="margin:0px; padding:0px"><code>ibm_is_security_group_rule</code></li><li style="margin:0px; padding:0px"><code>ibm_is_ipsec_policy</code></li><li style="margin:0px; padding:0px"><code>ibm_is_ike_policy</code></li><li style="margin:0px; padding:0px"><code>ibm_is_volume</code></li><li style="margin:0px; padding:0px"><code>ibm_is_public_gateway</code></li></ul>|[View code snippet](https://github.com/IBM-Cloud/terraform-provider-ibm/tree/master/examples/ibm-is-ng)|





