# Deploy Azure Cosmos DB MongoDB Cluster monitoring
This terraform script will deploy the following monitoring alerts for a Cosmos DB MongoDB Cluster

1. Resource Health  
Resource Health status is no longer 'Available'

2. Committed Memory high  
Whenever the average Committed Memory percent is greater than 90%

2. Committed Memory critical  
Whenever the average Committed Memory percent is greater than 98%

3. CPU Percent high  
Whenever the average CPU percent is greater than 90%

3. CPU Percent critical  
Whenever the average CPU percent is greater than 98%

4. Storage Percent over 80%  
Whenever the average storage percent is greater than 80%

5. Storage Percent over 90%  
Whenever the average storage percent is greater than 90%

6. Storage Percent over 95%  
Whenever the average storage percent is greater than 95%
