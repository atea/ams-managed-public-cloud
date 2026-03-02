# Documentation for Managed Azure Networking monitoring

The purpose of this document is to list and document currently supported services for Azure Network monitoring and explain the overall design.

## Overall design

All monitoring templates will be deployed in a dedicated Resource Group, per Azure Subscription.  
Resource Group default name: `RG-AMS-Monitoring-001`  
Every Azure Subscription with monitored resources will have dedicated Resource Group  
Every Azure Subscription will have dedicated Action Group  
Action Group default name: `AG-AMS-Monitoring-001`  
Action Group default short name: `AMS-Monitor`  
For every monitored resource, an Alert Rule will be created per alert type.  

Example: Azure Event Hub has 5 different alert types, thus 5 alert rules will be created.  

Resource Health Alerts are created per resource type, per subscription.  

## Alert flow

![Drawing describing the alert flow](./../../../Monitoring%20drawing.png)

## List of supported resource types

Select any of the links below to list the monitoring templates deployed for the resource.  

[Azure Application Gateway](./../Managed_Application_Gateway/)  
[Azure Network Connections](./../Managed_Azure_Connections/)  
[Azure DNS Private Zones](./../Managed_Azure_DNS_Private_Zones/)  
[Azure DNS Zones](./../Managed_Azure_DNS_Zones/)  
[Azure Firewall](./../Managed_Azure_Firewall/)  
[Azure Bastion Hosts](./../Managed_Bastion_Host/)  
[Azure Express Route Circuits](./../Managed_Expressroute_Circuits/)  
[Azure Express Route Gateways](./../Managed_Expressroute_Gateway/)  
[Azure Express Route Ports](./../Managed_Expressroute_Ports/)  
[Azure Front Doors](./../Managed_Front_Doors/)  
[Azure Load Balancers](./../Managed_Load_Balancers/)  
[Azure NAT Gateways](./../Managed_NAT_Gateways/)  
[Azure Network Security Groups](./../Managed_Network_Security_Groups/)  
[Azure Public IP Addresses](./../Managed_Public_IP_Addresses/)  
[Azure Route Tables](./../Managed_Route_Tables/)  
[Azure Traffic Manager Profiles](./../Managed_Traffic_Manager_Profiles/)  
[Azure Virtual Network Gateways](./../Managed_Virtual_Network_Gateways/)  
[Azure Virtual Networks](./../Managed_Virtual_Networks/)  
[Azure VPN Gateways](./../Managed_VPN_Gateways/)  
