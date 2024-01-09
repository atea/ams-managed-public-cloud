# Documentation for AMS Managed PaaS monitoring

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

[Azure Storage Accounts](./modules/Managed_StorageAccount/)  
[Azure Key Vault](./modules/Managed_Key_Vault/)  
[Azure App Service Plans](./modules/Managed_App_Services_Plan/)  
[Azure Web Apps](./modules/Managed_Web_App/)  
[Azure Application Gateways](./modules/Managed_Application_Gateway/)  
[Azure Data Factory](./modules/Managed_Data_Factory/)  
[Azure Event Hub](./modules/Managed_Event_Hub/)  
[Azure Load Balancer](./modules/Managed_Load_Balancer/)  
[Azure IoT Hub](./modules/Managed_IoT_Hub/)  
[Azure SQL Database](./modules/Managed_SQL_Database/)  
[Azure API Management](./modules/Managed_API_Management/)  
[Azure Cache for Redis](./modules/Managed_Redis_Cache/)  
[Azure Recovery Services Vault](./modules/Managed_Recovery_Services_Vault/)  
[Azure Service Bus Namespace](./modules/Managed_Service_Bus_Namespace/)  
[Azure Cosmos DB PostgreSQL Cluster](./modules/Managed_Cosmos_DB/Managed_Cosmos_DB_PostgreSQL/)  
[Azure Cosmos DB Mongo Database Account](./modules/Managed_Cosmos_DB/Managed_Cosmos_DB_MongoDB_Database_Account/)  
[Azure Cosmos DB Mongo Cluster](./modules/Managed_Cosmos_DB/Managed_Cosmos_DB_MongoDB_Cluster/)  
[Azure Cosmos DB NoSQL Account](./modules/Managed_Cosmos_DB/Managed_Cosmos_DB_NoSQL/)  
[Azure Cosmos DB Table](./modules/Managed_Cosmos_DB/Managed_Cosmos_DB_Table/)  
[Azure Cosmos DB Apache Cassandra](./modules/Managed_Cosmos_DB/Managed_Cosmos_DB_Apache_Cassandra/)  
[Azure Cosmos DB Apache Gremlin](./modules/Managed_Cosmos_DB/Managed_Cosmos_DB_Apache_Gremlin/)  
[Azure Logic App, App Services](./modules/Managed_Logic_App/App_Services/)  
[Azure Logic App, Consumption Based](./modules/Managed_Logic_App/Consumption_Based/)  
[Azure Function App](./modules/Managed_Function/web_app/)  
[Azure Analysis Services Server](./modules/Managed_Analysis_Services/)  
[Azure Front Door](./modules/Managed_Front_Door/)  
[Azure SQL Elastic Pool](./modules/Managed_SQL_Elastic_Pool/)  
[Azure Stream Analytics job](./modules/Managed_Stream_Analytics_job/)  
