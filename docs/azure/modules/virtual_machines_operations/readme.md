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

[Azure Virtual Machine](./../Managed_Virtual_Machine/)  
[Azure Virtual Machine Scale Sets](./../Managed_Virtual_Machine_Scalesets)