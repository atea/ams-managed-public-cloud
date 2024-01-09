# Deploy Azure Cosmos DB Table monitoring
This terraform script will deploy the following monitoring alerts for a Cosmos DB Table

1. Resource Health  
Resource Health status is no longer 'Available'

2. Total Requests  
Whenever the count Total Requests is greater or less than dynamic criteria

3. Normalized RU Consumption high  
Whenever the maximum Normalized RU Consumption is greater than 90%

3. Normalized RU Consumption critical  
Whenever the maximum Normalized RU Consumption is greater than 90%

4. Service Availability  
Whenever the average Service Availability is less than 100%




