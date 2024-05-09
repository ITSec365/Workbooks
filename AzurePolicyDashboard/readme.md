# Azure Policy Dashboard 

Azure Policy Dashboard provides you a unified view and full visibility to your azure policy deployments in Azure. 

Our newly dashboard is based on Azure Resource Graph (ARG) queries and divided to several sections such as:

-	**Policy Coverage:** summary view of all your Azure policies assigned, Policy definitions and Assignment mapping , List of custom policies  
-	**Policy Status:** policy compliance status  
-	**Policy Exemption Status:** List of policies with exemptions 
-	**Policy Actions:** filtered view of changes performed in azure policy, resource deployments denied by policy, resource deployments performed by policy from Azure Activity Logs 
(Log Source: Azure Activity Logs. Ensure respective Log Analytics Workspace is selected in the filter at the top of the workbook)



## Try it on the Azure Portal

To deploy the new workbook into your Microsoft Defender for Cloud console, click on *Deploy to Azure* for Azure Public cloud or *Deploy to Azure Gov* for government cloud.
During the deployment, you must select a subscription and resource group to store the report. 

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FITSec365%2FWorkbooks%2Fmain%2FAzurePolicyDashboard%2FAzurePolicyDashboardv1.json" target="_blank"><img src="https://aka.ms/deploytoazurebutton"/></a>
<a href="https://portal.azure.us/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FITSec365%2FWorkbooks%2Fmain%2FAzurePolicyDashboard%2FAzurePolicyDashboardv1.json" target="_blank"><img src="https://aka.ms/deploytoazuregovbutton"/></a>



#### Change Log 

|Date|Description|
|---|---|
|May-09-2024| Public availability of the workbook| 

