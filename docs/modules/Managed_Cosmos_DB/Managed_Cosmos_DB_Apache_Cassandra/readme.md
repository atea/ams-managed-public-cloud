# Deploy Azure Cosmos DB Apache Cassandra monitoring
This terraform script will deploy the following monitoring alerts for a Cosmos DB Apache Cassandra

1. Resource Health  
Resource Health status is no longer 'Available'

2. Normalized RU Consumption over 90%  
Whenever the maximum Normalized RU Consumption is greater than 90%

3. Normalized RU Consumption over 98%  
Whenever the maximum Normalized RU Consumption is greater than 98%

4. Service Availability  
Whenever the average Service Availability is less than 100%




