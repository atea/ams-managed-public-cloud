# Deploy Azure Cosmos DB PostgreSQL monitoring
This terraform script will deploy the following monitoring alerts for a Cosmos DB PostgreSQL

1. Resource Health  
Resource Health status is no longer 'Available'

2. CPU Percent high  
Whenever the average CPU percent is greater than 90%

2. CPU Percent critical  
Whenever the average CPU percent is greater than 90%

3. Memory Percent high  
Whenever the average Memory percent is greater than 90%

3. Memory Percent critical  
Whenever the average Memory percent is greater than 90%

4. Storage Percent over 80%  
Whenever the average storage percent is greater than 80%

5. Storage Percent over 90%  
Whenever the average storage percent is greater than 90%

6. Storage Percent over 95%  
Whenever the average storage percent is greater than 95%

7. IOPS Consumed Percentage  
Whenever the average VM Cached IOPS Consumed Percentage is greater than 90%




