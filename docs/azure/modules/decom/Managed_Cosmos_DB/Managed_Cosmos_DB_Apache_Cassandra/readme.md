# Deploy Azure Cosmos DB Apache Cassandra monitoring
## This terraform script will deploy the following monitoring alerts for a Cosmos DB Apache Cassandra

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**  
***The alert priority level is 2***  

2. Normalized RU Consumption* High  
Whenever the maximum Normalized RU* Consumption* is greater than 90%.  
**This indicates that database resources are approaching maximum utilization, potentially affecting application performance and scalability.**  
***The alert priority level is 3***  

3. Normalized RU* Consumption* Critical  
Whenever the maximum Normalized RU Consumption* is greater than 98%.  
**This signifies a critical situation where database resources are nearing full capacity, posing a risk of performance degradation and potential service disruptions.**  
***The alert priority level is 2***  

4. Service Availability  
Whenever the average Service Availability is less than 100%.  
**This alerts to situations where the service may experience downtime or interruptions, impacting user access and business operations.**  
***The alert priority level is 2***  

    > *Normalized RU Consumption refers to the amount of Request Units (measured in Request Units per second) consumed by a database operation, adjusted to a standardized scale for comparison across different databases and workloads.




