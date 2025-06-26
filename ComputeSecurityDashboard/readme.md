# Compute Security Dashboard for Microsoft Defender for Cloud

The new compute security dashboard for Microsoft Defender for Cloud provides you a unified view and full visibility to your virtual machine (VM) resources in Azure. If you have been actively using Azure virtual machines with  Microsoft Defender for Cloud in Azure, this workbook is for you!

Our newly dashboard is based on Azure Resource Graph (ARG) queries and divided to several sections such as:

-	**Virtual Machine Inventory:** summary view of all your Azure virtual machine and Arc resources for selected subscription(s) with OS, size, powerstate, SKU details 
-	**Orphaned Assets:** Orphaned VM components like Disks, NICs, Availability Sets, Public IPs, NSGs (not attached to any VMs) 
-	**Virtual Machine Status:** VMs not having Managed Disks, VMs with pending reboot status, VMs shut down with their compliance status, List of extension in VMs and Azure Arc Servers 
-	**Security Center recommendations:** filtered view of all Microsoft Defender for Cloud compute related recommendations including resource count, severity, and security control. **System Updates:** VMs missing system updates and filtered view of missing update details for selected VM 
-	**Service Principal:** List of Service Principals, Resources with System Assigned Identity , Resources with User Assigned Identity
-	**Backup:** VMs missing backup configurations and filtered view of back up jobs and backup alert details for selected subscription
-	**Encryption:** VMs not having managed disks and filtered view of disk encryption status
-	**Resource Changes:**  Configurations changes,updates and deletion in the last 14 days for the selected subscription
-	**Subscription RBAC:** Provides principals assigned with same role and same scope, principals with same role at multiple levels, principals with multiple roles
-	**Network:** Provides VMs deployed in subnets without Route tables and in subnets without NSGs. 


Informational options: using the action bars at the top section, select FAQ button to show the frequently asked questions. You can also see recent changes documented on the change log option.

## Try it on the Azure Portal

To deploy the new workbook into your Microsoft Defender for Cloud console, click on *Deploy to Azure* for Azure Public cloud or *Deploy to Azure Gov* for government cloud.
During the deployment, you must select a subscription and resource group to store the report. 

<a href="https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FITSec365%2FWorkbooks%2Fmain%2FComputeSecurityDashboard%2FComputeSecurityDashboardv5.json" target="_blank"><img src="https://aka.ms/deploytoazurebutton"/></a>
<a href="https://portal.azure.us/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2FITSec365%2FWorkbooks%2Fmain%2FComputeSecurityDashboard%2FComputeSecurityDashboardv5.1.json" target="_blank"><img src="https://aka.ms/deploytoazuregovbutton"/></a>

### Demo
![Dashboard demo](./compsec.GIF)

#### Change Log 

|Date|Description|
|---|---|
|April-21-2022| Public availability of the workbook| 
|Nov-2-2022| Updated Orphaned Resources  | 
|June-6-2023| Added Azure Arc inventory, Service Principals and backup details  | 
|July-31-2023| Added Encryption, Resource Changes and Subscription RBAC  |
|October-11-2023| Added Network section  |
|June-10-2025| Added VM Image details in VM Inventory  |

### Upcoming changes


