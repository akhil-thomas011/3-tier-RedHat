# 3-Tier Red HAt on Azure 
## Solution Overview 
This Azure Quick Start template deploys a 3 Tier Red Hat Solution on Azure.  The Solution includes Presentation Tier Web Servers, Application tier App Servers and Data Tier Database Servers running Red Hat Enterprise Linux 7.3. Template will build everything starting from Azure Infrastructure components to Red Hat VMs deployment. This template will deploy multiple number of VMs in each tier as per requirement. 

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fakhil-thomas011%2F3-tier-RedHat%2Fmaster%2Fazuredeploy.json" target="_blank">
<img src="https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/deploytoazure.png"/>
</a>
<a href="http://armviz.io/#/?load=https%3A%2F%2Fraw.githubusercontent.com%2Fakhil-thomas011%2F3-tier-RedHat%2Fmaster%2Fazuredeploy.json" target="_blank">
<img src="https://raw.githubusercontent.com/Azure/azure-quickstart-templates/master/1-CONTRIBUTION-GUIDE/images/visualizebutton.png"/>
</a> 
 

##Deployment Solution Architecture 

This template will deploy: 

- Four storage account 
-	One Virtual Network with four subnets
-	External Load Balancer to load balance all the Web VMs and to facilitate access to them.
- Internal Load Balancer to load balance all the App VMs.
-	2 Public IP’s, one for external Load balancer and other for Jump VM. 
-	3 Virtual Machine Availability sets for Presentation Tier, Application Tier and Data tier.
-	One Jump VM.
-	Two Red Hat Enterprise Linux VMs in each tier.

![Deployment Solution Architecture](https://github.com/SpektraSystems/barracuda-waf-solution/blob/master/images/barracuda-architecture.png?raw=true)

##Licenses and Costs 

This Barracuda Web Application Firewall is the PAYG model and doesn't require the user to license it, it will be licensed automatically after the instance is launched first time and user will be charged hourly for Barracuda Web Application Firewall Software on Microsoft. Click [here](https://azure.microsoft.com/en-us/marketplace/partners/barracudanetworks/waf/#hourly) for pricing details.

##Prerequisites 

- Azure Subscription with specified payment method (Barracuda WAF is a market place product and requires payment method to be specified in Azure Subscription
-	User account with admin or contributor access to the given azure subscription

##Deployment Steps  

Build your Barracuda WAF environment on Azure in a few simple steps:  
- Launch the Template by click on Deploy on Azure.  
- Fill in all the required parameter values. Accept the terms and condition on click Purchase. The deployment takes about 30 minutes. 
- Follow the post deployment configuration document [here](https://github.com/SpektraSystems/barracuda-waf-solution/blob/master/images/barracuda-waf-post-deployment-configuration-guide.pdf) for further configuration. 

##Support 

For any support related questions or customization requirements, please contact info@spektrasystems.com



