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

![Drawing describing the alert flow](./../../../Monitoring%20drawing.png)

## List of supported resource types

Select any of the links below to list the monitoring templates deployed for the resource.  

[Azure Analysis Services](./../Managed_Analysis_Services/)  
[Azure API Management](./../Managed_API_Management/)  
[Azure App Service](./../Managed_App_Service/)  
[Azure App Service Plan](./../Managed_App_Services_Plan/)  
[Azure Application Gateway](./../Managed_Application_Gateway/)  
[Azure Application Insights](./../Managed_Application_Insights/)  
[Azure Automation Account](./../Managed_Automation_Account/)  
[Azure Cache for Redis](./../Managed_Redis_Cache/)  
[Azure Cosmos DB](./../Managed_Cosmos_DB/)  
[Azure Data Factory](./../Managed_Data_Factory/)  
[Azure Event Hub](./../Managed_Event_Hub/)  
[Azure Front Door](./../Managed_Front_Door/)  
[Azure Function App](./../Managed_App_Service/)  
[Azure IoT Hub](./../Managed_IoT_Hub/)  
[Azure Key Vault](./../Managed_Key_Vault/)  
[Azure Load Balancer](./../Managed_Load_Balancer/)  
[Azure Logic App](./../Managed_Logic_App/)  
[Azure Recovery Services Vault](./../Managed_Recovery_Services_Vault/)  
[Azure Service Bus Namespace](./../Managed_Service_Bus_Namespace/)  
[Azure SQL Database](./../Managed_SQL_Database/)  
[Azure SQL Elastic Pool](./../Managed_SQL_Elastic_Pool/)  
[Azure Storage Account](./../Managed_StorageAccount/)  
[Azure Stream Analytics job](./../Managed_Stream_Analytics_job/)  
[Azure Event Grid](./../Managed_Event_Grid/)  
[Azure Container Instance (Update Pending)](./../Managed_Container_Instance)  
[Azure Container Apps](./../Managed_Container_Apps)  
[Azure Kubernetes Service (Update Pending)](./../Managed_Kubernetes_Service)  