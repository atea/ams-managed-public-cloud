# Deploy Azure Cosmos DB NoSQL monitoring
This terraform script will deploy the following monitoring alerts for a Cosmos DB NoSQL

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**  
***The alert priority level is 2***  

2. Region Failed  
Whenever the count Region Failed Over is greater than 0.  
**This indicates instances where a region has experienced a failover event, potentially affecting service availability and requiring attention to ensure seamless operation.**  
***The alert priority level is 3***  

3. Total Requests  
Whenever the count Total Requests is greater or less than dynamic criteria.  
**This alerts to situations where there's a significant variation in the number of requests, which may indicate changes in user activity or system behavior.**  
***The alert priority level is 5***  

4. Normalized RU Consumption High  
Whenever the maximum Normalized RU Consumption* is greater than 90%.  
**This indicates that database resources are nearing their maximum capacity, potentially impacting performance and scalability.**  
***The alert priority level is 3***  

5. Normalized RU Consumption Critical  
Whenever the maximum Normalized RU Consumption* is greater than 98%.  
**This signifies a critical situation where database resources are severely strained, likely leading to performance degradation and service disruptions.**  
***The alert priority level is 2***  

6. Service Availability  
Whenever the average Service Availability is less than 100%.  
**This alerts to instances where the service may experience downtime or interruptions, affecting user access and business continuity.**  
***The alert priority level is 2***  

7. Region Offlined  
Whenever the count Region Offlined is greater than 0.  
**This indicates situations where a region has become unavailable, potentially disrupting service availability and requiring immediate attention.**  
***The alert priority level is 3***  

8. Dedicated Gateway Average CPU** Usage High  
Whenever the average DedicatedGatewayAverageCPUUsage is greater than 90%.  
**This indicates increased demand or workload on the dedicated gateway, potentially affecting performance and requiring resource optimization.**  
***The alert priority level is 3***  

9. Dedicated Gateway Average CPU** Usage Critical  
Whenever the average DedicatedGatewayAverageCPUUsage is greater than 98%.  
**This signifies a critical situation where the dedicated gateway is severely strained, possibly leading to performance degradation and service interruptions.**  
***The alert priority level is 2***  

10. SQL Database Deleted  
Whenever the SQL Database is Deleted.  
**This indicates instances where a SQL database has been removed intentionally, potentially affecting data availability and requiring investigation to ensure proper data management.**  
***The alert priority level is 2***  

    > *Normalized RU Consumption refers to the amount of Request Units (measured in Request Units per second) consumed by a database operation, adjusted to a standardized scale for comparison across different databases and workloads.  
    > **CPU stands for Central Processing Unit. It is often referred to as the "brain" of the computer because it performs most of the processing inside a computer.







