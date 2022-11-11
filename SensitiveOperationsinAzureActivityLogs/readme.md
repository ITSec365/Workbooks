# Sensitive Operations in Azure Activity Logs 

 This Workbook utilizes Azure Activity Logs as a data source and it can be used to monitor sesitive operations from security aspects and to review who performed it and from which IP. These operations are idenified based on CIS Azure Foundation Benchmark and common techniques used in Azure security attacks as identified in Azure Threat Research Matrix (ATRM). 


This workbook provides filtered view of Azure Activity Logs and is divided to several sections such as:

-	**Overall:**  filtered view of administrative activities performed by various callers   
-	**Compute:** filtered View of Activity Log events related to VM Extension Changes, VM Run commands and VM Local adminpassword reset, VM Public IP assignments, AKS Run commands 
-	**Network:** filtered View of Activity Log events related to NSG Rule changes, Azure DNS changes, Network port changes  
-	**Policy:** filtered View of Activity Log events related to Policy changes, Resource lock changes, deployments denied by Azure Policy and deployments performed by Azure Policy 
-	**Security:** filtered View of Activity Log events related to Sentinel Analytic Rule changes, Data connector changes, workbook changes, Log alert changes, Diagnostic setting changes, 
-	**Data:** filtered View of Activity Log events related to Azure SQL changes, storage account changes, Key Vault changes 
-	**Account:** filtered View of Activity Log events related to Azure resource role changes  
-	**Application:** filtered View of Activity Log events related to App Service changes, Function App, Logic App, Automation Account Webhooks 
-	**External Access:** filtered View of Activity Log events related to Light House Registration Assignments, Guest Account activities 

Please refer to this blog for more details- https://itsec365.wordpress.com/2022/08/02/reviewing-azure-activity-logs/

## Try it on the Azure Portal

To deploy the new workbook into your Microsoft Defender for Cloud console, click on *Deploy to Azure* for Azure Public cloud or *Deploy to Azure Gov* for government cloud.
During the deployment, you must select a subscription and resource group to store the workbook. 

<a  href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FITSec365%2FWorkbooks%2Fmain%2FSensitiveOperationsinAzureActivityLogs%2FSensitiveOperationsinAzureActivityLogReview.json" target="_blank"><img src="https://aka.ms/deploytoazurebutton"/></a>
<a href="https://portal.azure.us/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FITSec365%2FWorkbooks%2Fmain%2FSensitiveOperationsinAzureActivityLogs%2FSensitiveOperationsinAzureActivityLogReview.json" target="_blank"><img src="https://aka.ms/deploytoazuregovbutton"/></a>

### Demo
![Workbook demo](./Activity.GIF)

#### Change Log 

|Date|Description|
|---|---|
|Aug-2-22| Public availability of the workbook| 
|Aug-26-22| Added AKS, Function Apps,LogicApps,Webhooks and Webjobs per Azure Threat Research Matrix detections  | 
|Oct-4-22| Added External Access  | 
|Nov-11-22| Updated Caller Activities section  | 
