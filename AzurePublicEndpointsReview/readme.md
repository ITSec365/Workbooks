# Azure Public Endpoints Review Workbook 

This workbook uses Azure Resource Graph and Azure Rest API to pull real time data from the selected subscriptions.  This workbook can be used to review the Azure resources which are publicly available or exposed to internet. 

This workbook provides filtered view of Azure Resources and Network configurations and is divided to several sections such as:

-	**PaaS Services:**  filtered view listing various PaaS Services (Storage Account, Key vault, Event Hub, App Services, Databases) with Public Access Property status     
-	**Network Rules:** filtered View listing Public IPs with assignment status, Network rules configured in various network services like Application Gateway, Front Door, Firewall etc. 
-	**Network Services: ** filtered View listing Network services like Bastion Hosts, VNet Gateways, VPN Gateways etc.   
-	**API Connections: ** filtered View listing API Connections and Logic App Workflows
-	**Internal Networks: ** filtered View listing VNet configurations, Route tables, NSG Rules  
-	**MDC Recommendations: ** filtered View listing Public Access related recommendations for VM, PaaS services and Data in transit security recommendations

Please refer to this blog for more details- 

## Try it on the Azure Portal

To deploy the new workbook into your Microsoft Defender for Cloud console, click on *Deploy to Azure* for Azure Public cloud or *Deploy to Azure Gov* for government cloud.
During the deployment, you must select a subscription and resource group to store the workbook. 

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FITSec365%2FWorkbooks%2Fmain%2FAzurePublicEndpointsReview%2FAzurePublicEndpointsReview.json" target="_blank"><img src="https://aka.ms/deploytoazurebutton"/></a>
<a href="https://portal.azure.us/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FITSec365%2FWorkbooks%2Fmain%2FAzurePublicEndpointsReview%2FAzurePublicEndpointsReview.json" target="_blank"><img src="https://aka.ms/deploytoazuregovbutton"/></a>

### Demo
![Workbook demo](./Activity.GIF)

#### Change Log 

|Date|Description|
|---|---|
|March-3-23| Public Preview of the workbook| 
