# Microsoft-Azure
* **Delete** means authorized users can still read and modify a resource, but they can't delete the resource.
* **ReadOnly** means authorized users can read a resource, but they can't delete or update the resource. Applying this lock is similar to restricting all authorized users to the permissions granted by the Reader role.

# Microsoft Azure Fundamentals: Describe cloud concepts
![shared-responsibility-b3829bfe](https://github.com/user-attachments/assets/e7f44629-09f5-4671-aa3e-557d4b7aed19)

# Azure Arc
Azure Arc is a set of technologies that helps manage your cloud environment.

# Describe the consumption-based model

*  Capital expenditure (CapEx) 
CapEx is typically a one-time, up-front expenditure to purchase or secure tangible resources. A new building, repaving the parking lot, building a datacenter, or buying a company vehicle are examples of CapEx.

*  Operational expenditure (OpEx) 
 OpEx is spending money on services or products over time. Renting a convention center, leasing a company vehicle, or signing up for cloud services are all examples of OpEx.

* Cloud computing falls under OpEx

# Scalability
 Scalability refers to the ability to adjust resources to meet demand.
 
# Vertical scaling
you could vertically scale up to add more CPUs or RAM to the virtual machine

# Horizontal scaling
 if you suddenly experienced a steep jump in demand, your deployed resources could be scaled out (either automatically or manually). 

# Compare the Pricing and Total Cost of Ownership calculators

* TCO calculator -  designed to help you compare the costs for running an on-premises infrastructure compared to an Azure Cloud infrastructure

To migrate to Azure, you might:

Use Azure Virtual Machines instances, similar to the virtual machines used in your datacenter.
Use Azure Application Gateway for load balancing.
Use Azure SQL Database to hold inventory and pricing information.

In practice, you would define your requirements in greater detail. But here are some basic facts and requirements to get you started:

The application is used internally. It's not accessible to customers.
This application doesn't require a massive amount of computing power.
The virtual machines and the database run all the time (730 hours per month).
The network processes about 1 TB of data per month.
The database doesn't need to be configured for high-performance workloads and requires no more than 32 GB of storage.

# Explore the Pricing Calculator
* Products This is where you choose the Azure services that you want to include in your estimate. You'll likely spend most of your time here.
* Example scenarios Here you'll find several reference architectures, or common cloud-based solutions that you can use as a starting point.
* Saved estimates Here you'll find your previously saved estimates.
* FAQs Here you'll discover answers to frequently asked questions about the Pricing calculator.

# What is Cost Management?
* Cost Management provides the ability to quickly check Azure resource costs, create alerts based on resource spend, and create budgets that can be used to automate management of resources. Cost analysis is a subset of Cost Management that provides a quick visual for your Azure costs.

# Cost alerts
* Budget alerts - Budget alerts notify you when spending, based on usage or cost, reaches or exceeds the amount defined in the alert condition of the budget.
* Credit alerts - notify you when your Azure credit monetary commitments are consumed.
* Department spending quota alerts - notify you when department spending reaches a fixed threshold of the quota.
* Budgets - A budget is where you set a spending limit for Azure. You can set budgets based on a subscription, resource group, service type, or other criteria.

  # Describe the purpose of tags -Tags provide extra information, or metadata, about your resources. 
* Resource management Tags enable you to locate and act on resources that are associated with specific workloads, environments, business units, and owners.
* Cost management and optimization Tags enable you to group resources so that you can report on costs, allocate internal cost centers, track budgets, and forecast estimated cost.
* Operations management Tags enable you to group resources according to how critical their availability is to your business. This grouping helps you formulate service-level agreements (SLAs). An SLA is an uptime or performance guarantee between you and your users.
* Security Tags enable you to classify data by its security level, such as public or confidential.
* Governance and regulatory compliance Tags enable you to identify resources that align with governance or regulatory compliance requirements, such as ISO 27001. Tags can also be part of your standards enforcement efforts. For example, you might require that all resources be tagged with an owner or department name.
* Workload optimization and automation Tags can help you visualize all of the resources that participate in complex deployments. For example, you might tag a resource with its associated workload or application name and use software such as Azure DevOps to perform automated tasks on those resources.

# How do I manage resource tags?
* You can add, modify, or delete resource tags through Windows PowerShell, the Azure CLI, Azure Resource Manager templates, the REST API, or the Azure portal.

# Describe the purpose of Microsoft Purview
![purview-solution-areas-ceb1bedf](https://github.com/user-attachments/assets/f8b23c80-2d4b-44d9-a9cb-f70e022d7984)

# Types of Resource Locks

**A resource lock prevents resources from being accidentally deleted or changed.**

# Azure Cloud Shell

Azure Cloud Shell is a browser-based shell tool that allows you to create, configure, and manage Azure resources using a shell. Azure Cloud Shell support both Azure PowerShell and the Azure Command Line Interface (CLI), which is a Bash shell.

# What is Azure PowerShell?
Azure PowerShell is a shell with which developers, can run commands called command-lets (cmdlets). These commands call the Azure REST API to perform management tasks in Azure.

# Describe the purpose of Azure Arc

In utilizing Azure Resource Manager (ARM), Arc lets you extend your Azure compliance and monitoring to your hybrid and multi-cloud configurations. Azure Arc simplifies governance and management by delivering a consistent multi-cloud and on-premises management platform.

Azure Arc provides a centralized, unified way to:

Manage your entire environment together by projecting your existing non-Azure resources into ARM.
Manage multi-cloud and hybrid virtual machines, Kubernetes clusters, and databases as if they are running in Azure.
Use familiar Azure services and management capabilities, regardless of where they live.
Continue using traditional ITOps while introducing DevOps practices to support new cloud and native patterns in your environment.
Configure custom locations as an abstraction layer on top of Azure Arc-enabled Kubernetes clusters and cluster extensions.

# What can Azure Arc do outside of Azure?
Currently, Azure Arc allows you to manage the following resource types hosted outside of Azure:

* Servers
* Kubernetes clusters
* Azure data services
* SQL Server
* Virtual machines (preview)

**Azure Resource Manager (ARM) is the deployment and management service for Azure. It provides a management layer that enables you to create, update, and delete resources in your Azure account. Anytime you do anything with your Azure resources, ARM is involved.**

![image](https://github.com/user-attachments/assets/6e13848e-1492-4acc-9cc6-c2a2d3df51c6)

![image](https://github.com/user-attachments/assets/89396991-5883-4d49-8f8f-be8d97761712)

![image](https://github.com/user-attachments/assets/f3808120-0164-4def-8d6b-bb1b52eeb3ba)


# Describe the purpose of Azure Advisor
Azure Advisor evaluates your Azure resources and makes recommendations to help improve reliability, security, and performance, achieve operational excellence, and reduce costs. Azure Advisor is designed to help you save time on cloud optimization. The recommendation service includes suggested actions you can take right away, postpone, or dismiss.

# Describe Azure Service Health
. Azure Service Health helps you keep track of Azure resource, both your specifically deployed resources and the overall status of Azure. Azure service health does this by combining three different Azure services:

* Azure Status is a broad picture of the status of Azure globally. Azure status informs you of service outages in Azure on the Azure Status page. The page is a global view of the health of all Azure services across all Azure regions. It’s a good reference for incidents with widespread impact.
* Service Health provides a narrower view of Azure services and regions. It focuses on the Azure services and regions you're using. This is the best place to look for service impacting communications about outages, planned maintenance activities, and other health advisories because the authenticated Service Health experience knows which services and resources you currently use. You can even set up Service Health alerts to notify you when service issues, planned maintenance, or other changes may affect the Azure services and regions you use.
* Resource Health is a tailored view of your actual Azure resources. It provides information about the health of your individual cloud resources, such as a specific virtual machine instance. Using Azure Monitor, you can also configure alerts to notify you of availability changes to your cloud resources.

# Describe Azure Monitor
Azure Monitor can monitor Azure resources, your on-premises resources, and even multi-cloud resources like virtual machines hosted with a different cloud provider.

![azure-monitor-overview-614cd2fd](https://github.com/user-attachments/assets/67abc99e-e383-4b6f-be1f-a048f5723ed0)

![image](https://github.com/user-attachments/assets/ec90ac43-00bb-440c-9888-bec662d9bc0e)

![image](https://github.com/user-attachments/assets/57eba540-5b28-4905-ba2a-2f6e3be89a0a)

![account-scope-levels-9ceb3abd](https://github.com/user-attachments/assets/cbdbbd2a-039f-4362-9a00-c9aa4625be0f)
A region is a geographical area on the planet that contains at least one, but potentially multiple datacenters that are nearby and networked together with a low-latency network

![availability-zones-c22f95a3](https://github.com/user-attachments/assets/a40a1ade-b733-492b-9dd8-e27f7da1a6ac)
Availability zones are physically separate datacenters within an Azure region. Each availability zone is made up of one or more datacenters equipped with independent power, cooling, and networking.

![region-pairs-7c495a33](https://github.com/user-attachments/assets/a69e6879-31d4-44ae-a1d5-cd558de1cee7)
![subscriptions-d415577b](https://github.com/user-attachments/assets/b3f12d88-6fb7-4543-aa32-ea2a9a3a5c51)
![management-groups-subscriptions-dfd5a108](https://github.com/user-attachments/assets/8b197c8a-611a-47ec-a83c-da7ee756d0b5)
























