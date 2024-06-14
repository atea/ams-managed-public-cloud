# Documentation for Managed Azure Platform monitoring

The purpose of this document is to list and document currently supported services for Azure PaaS monitoring and explain the overall design.

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

![Drawing describing the alert flow](./Monitoring%20drawing.png)

## List of supported resource types

Select any of the links below to list the monitoring templates deployed for the resource.  

[Azure Analysis Services](./azure/modules/Managed_Analysis_Services/)  
[Azure API Management](./azure/modules/Managed_API_Management/)  
[Azure App Service](./azure/modules/Managed_App_Service/)  
[Azure App Service Plan](./azure/modules/Managed_App_Services_Plan/)  
[Azure Application Gateway](./azure/modules/Managed_Application_Gateway/)  
[Azure Application Insights](./azure/modules/Managed_Application_Insights/)  
[Azure Automation Account](./azure/modules/Managed_Automation_Account/)  
[Azure Cache for Redis](./azure/modules/Managed_Redis_Cache/)  
[Azure Cosmos DB](./azure/modules/Managed_Cosmos_DB/)  
[Azure Data Factory](./azure/modules/Managed_Data_Factory/)  
[Azure Event Hub](./azure/modules/Managed_Event_Hub/)  
[Azure Front Door](./azure/modules/Managed_Front_Door/)  
[Azure Function App](./azure/modules/Managed_App_Service/)  
[Azure IoT Hub](./azure/modules/Managed_IoT_Hub/)  
[Azure Key Vault](./azure/modules/Managed_Key_Vault/)  
[Azure Load Balancer](./azure/modules/Managed_Load_Balancer/)  
[Azure Logic App](./azure/modules/Managed_Logic_App/)  
[Azure Recovery Services Vault](./azure/modules/Managed_Recovery_Services_Vault/)  
[Azure Service Bus Namespace](./azure/modules/Managed_Service_Bus_Namespace/)  
[Azure SQL Database](./azure/modules/Managed_SQL_Database/)  
[Azure SQL Elastic Pool](./azure/modules/Managed_SQL_Elastic_Pool/)  
[Azure Storage Account](./azure/modules/Managed_StorageAccount/)  
[Azure Stream Analytics job](./azure/modules/Managed_Stream_Analytics_job/)  
[Azure Event Grid](./azure/modules/Managed_Event_Grid/)  

