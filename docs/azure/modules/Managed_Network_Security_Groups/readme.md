# Deploy Azure Network Security Group (NSG) monitoring
## This terraform script will deploy the following monitoring alerts for a Network Security Group

1. Activity Log Azure Network Security Group Delete  
Activity Log alert when deletion succeeds for Azure Network Security Group (operation: Microsoft.Network/networkSecurityGroups/delete).  
**Alerts if a NSG is successfully deleted. Azure NSG is a network security feature for filtering network traffic, that if deleted can impact function and security for multiple services in Azure.**  
***The alert priority level is 2***  
