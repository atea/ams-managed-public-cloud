# Deploy Azure Cosmos DB Apache Gremlin monitoring
This terraform script will deploy the following monitoring alerts for a Cosmos DB Apache Gremlin

1. Resource Health  
Resource Health status is no longer 'Available'

2. Region Failed  
Whenever the count Region Failed Over is greater than 0

3. Total Requests  
Whenever the count Total Requests is greater or less than dynamic criteria

4. Normalized RU Consumption High  
Whenever the maximum Normalized RU Consumption is greater than 90%

4. Normalized RU Consumption Critical  
Whenever the maximum Normalized RU Consumption is greater than 98%

5. Service Availability  
Whenever the average Service Availability is less than 100%

6. Region Offlined  
Whenever the count Region Offlined is greater than 0

1. Gremlin Database Deleted  
Whenever the count Gremlin Database Deleted is greater than 0







