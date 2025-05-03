# Azure Threat Research Matrix Workbook

This Workbook provides detection methods for various tactics & techniques used by threat actors to compromise an Azure resource or Entra ID. This workbook leverages detection methods provided in Azure Threat Research Matrix framework. This Workbook utilizes Azure Activity Logs and Entra ID Audit Logs as a data source. 

Objective of this workbook is to educate security professionals on various threat vectors to Azure resources when not following Azure Security Best Practices and their detection methods using ATRM framework. It is not intended to be complete list. Reference: https://techcommunity.microsoft.com/blog/microsoft-security-blog/introducing-the-azure-threat-research-matrix/3584976

Note a brief information is provided on top of each table for specific attack scenario. Please review them to get more information on attack scenarios.

This workbook provides filtered view of related log events from Azure Activity Logs and Entra ID Audit Logs for various attack scenarios as given below. Note most of these activities will be performed by IT Administrators. You need to review who is doing  this activity and from which IP address to identify any suspicious activities.  

|Tab|Attack vectors covered |
|---|---|
|Overall:| filtered view of administrative activities performed by various callers|
|Compute:|  Deploying malicious VM Extension, Deploying malicious Gallery Application,  Abusing VM Run commands , VM Local admin password reset, Exporting VM Disk using SAS URI , VM Disk snapshot, VM Serial Console Access,  AKS Cluster Command Invoke, VM Public IP assignments |
|Network:| Network configuration tampering like NSG Rule changes, Azure DNS changes, Network port changes |
|Policy:|  Azure Policy modification for persistence , Resource lock changes, Resource deployments denied by Azure Policy and deployments performed by Azure Policy|
|Security:| Tampering sentinel or log collection settings like  Sentinel Analytic Rule changes, Data connector changes, workbook changes, Log alert changes, Diagnostic setting changes|
|Data:| Data exfiltration or data sabotage attacks related to Azure SQL changes, storage account changes, Key Vault changes|
|Subscription:| Privilege Escalation (Azure RBAC and cloud shell) , Subscription hijacking, Adding new subscription or management group changes|
|Application:| Remote triggering App Services , Logic Apps or automation accounts using HTTP triggers or webhooks and resource level changes|
|External Access:| Suspicious External user activities using Azure Light House or Guest Accounts|
|Identity:| Consent to Malicious Application , Privileged Role Activation,Using RBAC Elevate Access, Update Permission to Application, Update Certificates or Secrets to Application, Modify Security Info(MFA Methods), Abusing TAP, Tamper Conditional Access Policy, Modify User properties to join dynamic groups, Add accounts or Service principal, Add Rogue Device |


## Try it on the Azure Portal

To deploy the new workbook into your Microsoft Defender for Cloud console, click on *Deploy to Azure* for Azure Public cloud or *Deploy to Azure Gov* for government cloud.
During the deployment, you must select a subscription and resource group to store the workbook. 

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FITSec365%2FWorkbooks%2Fmain%2FAzureThreatResearchMatrixWorkbook%2FAzureThreatResearchMatrixWorkbook.json" target="_blank"><img src="https://aka.ms/deploytoazurebutton"/></a>
<a href="https://portal.azure.us/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FITSec365%2FWorkbooks%2Fmain%2FAzureThreatResearchMatrixWorkbook%2FAzureThreatResearchMatrixWorkbook.json" target="_blank"><img src="https://aka.ms/deploytoazuregovbutton"/></a>

### Demo
![Workbook demo](./identity.GIF)
![Workbook demo](./part3.GIF)

#### Change Log 

|Date|Description|
|---|---|
|May-1-25| Public availability of the workbook| 
