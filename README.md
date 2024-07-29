# Microsoft-Azure
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
