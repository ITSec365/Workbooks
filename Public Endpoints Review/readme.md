Contents of this workbook are: 
PaaS Services: Lists PaaS Services (Storage Account, Key vault, Event Hub, App Services, Databases) with Public Access Property status  
Network Rules: Lists Public IPs with assignment status, Network rules configured in various network services like Application Gateway, Front Door, Firewall etc. 
Network Services: Lists Resources like Bastion Hosts, VNet Gateways, VPN Gateways etc. 
API Connections: Lists API Connections and Logic App Workflows
Internal Networks: Lists VNet configurations, Route tables, NSG Rules 
MDC Recommendations: Lists Public Access related recommendations for VM, PaaS services and Data in transit security recommendations. 

Some of the Review Considerations while using this workbook are: 
PaaS Services
Review the Public network access for the respective resource and see if it meets your security requirements. For example, some of the storage accounts and databases containing sensitive data may be accidentally exposed to the internet.
Note App Services and Function Apps will have default public access (with null value in JSON) unless you specifically disable it. Review the HTTP Triggers and web jobs in app services to see if they have anonymous access. 

Network Rules
Review the resources with Public IP address
Review the Load Balancer, Application Gateway to see the backend pools connecting to Public IPs.
Review the Firewall rules with * (All IP addresses) or any unknown IP address in source or destination and sensitive ports like 3389, 22, 21 etc.
 

Network Services

Review the existing Bastion Hosts, VPN Gateways, VNet Gateways, Express Route Circuits

API Connection
Review the API Connection connecting Logic Apps to external SaaS apps

Internal Networks
Review the NSG rules with * (All IP addresses) in source or destination and sensitive ports like 3389, 22, 21 etc.
Review the Route Tables with internet destinations and nexthop without virtualappliances
Review Subnets without Route Tables

MDC Recommendations
Review the MDC Recommendations and assets and remediations for each recommendation. 
