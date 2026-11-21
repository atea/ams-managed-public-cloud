# Deploy Azure Cosmos DB Table monitoring
## This terraform script will deploy the following monitoring alerts for a Cosmos DB Table

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**  
***The alert priority level is 2***  

2. Total Requests  
Whenever the count Total Requests is greater or less than dynamic criteria.  
**This alerts to situations where there's a significant variation in the number of requests, which may indicate changes in user activity or system behavior.**  
***The alert priority level is 5***   

3. Normalized RU Consumption* High  
Whenever the maximum Normalized RU Consumption* is greater than 90%.  
**This indicates that database resources are nearing their maximum capacity, potentially impacting performance and scalability.**  
***The alert priority level is 3***  

3. Normalized RU Consumption* Critical  
Whenever the maximum Normalized RU Consumption* is greater than 98%.  
**This signifies a critical situation where database resources are severely strained, likely leading to performance degradation and service disruptions.**  
***The alert priority level is 2***  

4. Service Availability  
Whenever the average Service Availability is less than 100%.  
**This alerts to instances where the service may experience downtime or interruptions, affecting user access and business continuity.**  
***The alert priority level is 2***  

    > *Normalized RU Consumption refers to the amount of Request Units (measured in Request Units per second) consumed by a database operation, adjusted to a standardized scale for comparison across different databases and workloads.



