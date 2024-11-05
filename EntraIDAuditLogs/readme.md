# Entra ID Audit Log Hunting Workbook

Entra ID Audit Log Hunting workbook assists in identifying sensitive operations using Entra ID Audit  Logs. 

This Workbook utilizes Entra ID (Azure AD) Audit Logs as a data source and it can be used to monitor sensitive operations from security aspects. 
Suspecious activities in Azure Resources can be detected by reviewing who performed it and from which IP.
This workbook leverages detection methods provided in One Page Guide provided by Microsoft Incident response team. 
Link: https://www.microsoft.com/en-us/security/blog/2024/01/17/new-microsoft-incident-response-guides-help-security-teams-analyze-suspicious-activity/



## Try it on the Azure Portal

To deploy the new workbook into your Microsoft Defender for Cloud console, click on *Deploy to Azure* for Azure Public cloud or *Deploy to Azure Gov* for government cloud.
During the deployment, you must select a subscription and resource group to store the report. 

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FITSec365%2FWorkbooks%2Fmain%2FEntraIDAuditLogs%2FEntraIDAuditLogs.json" target="_blank"><img src="https://aka.ms/deploytoazurebutton"/></a>
<a href="https://portal.azure.us/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FITSec365%2FWorkbooks%2Fmain%2FEntraIDAuditLogs%2FEntraIDAuditLogs.json" target="_blank"><img src="https://aka.ms/deploytoazuregovbutton"/></a>



#### Change Log 

|Date|Description|
|---|---|
|November-05-2024| Public availability of the workbook| 
