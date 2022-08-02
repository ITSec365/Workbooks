# Sensitive Operations in Azure Activity Logs 

 This Workbook utilizes Azure Activity Logs as a data source and it can be used to monitor sesitive operations from security aspects and to review who performed it and from which IP. These operations are idenified based on CIS Azure Foundation Benchmark and common techniques used in Azure security attacks. 


This workbook provides filtered view of Azure Activity Logs and is divided to several sections such as:

-	**Overall:**  filtered view of administrative activities performed by various callers   
-	**Compute:** filtered View of Activity Log events related to VM Extension Changes, VM Run commands and VM Local adminpassword reset, VM Public IP assignments 
-	**Network:** filtered View of Activity Log events related to NSG Rule changes, Azure DNS changes, Network port changes  
-	**Policy:** filtered View of Activity Log events related to Policy changes, Resource lock changes, deployments denied by Azure Policy and deployments performed by Azure Policy 
-	**Security:** filtered View of Activity Log events related to Sentinel Analytic Rule changes, Data connector changes, workbook changes, Log alert changes, Diagnostic setting changes, 
-	**Data:** filtered View of Activity Log events related to Azure SQL changes, storage account changes, Key Vault changes 
-	**Account:** filtered View of Activity Log events related to Azure resource role changes  
-	**Application:** filtered View of Activity Log events related to App Service changes 



## Try it on the Azure Portal

To deploy the new workbook into your Microsoft Defender for Cloud console, click on *Deploy to Azure* for Azure Public cloud or *Deploy to Azure Gov* for government cloud.
During the deployment, you must select a subscription and resource group to store the report. 

<a  href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FITSec365%2FWorkbooks%2Fmain%2FSensitiveOperationsinAzureActivityLogs%2FSensitiveOperationsAzureActivity.json" target="_blank"><img src="https://aka.ms/deploytoazurebutton"/></a>
<a href="https://portal.azure.us/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FAzure%2FAzure-Security-Center%2Fmain%2FWorkbooks%2FWellArchitected%2520Framework%2520Security%2FarmTemplate.json" target="_blank"><img src="https://aka.ms/deploytoazuregovbutton"/></a>

![Workbook demo](./Activity.GIF)

