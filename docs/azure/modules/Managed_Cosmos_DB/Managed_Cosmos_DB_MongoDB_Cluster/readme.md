# Deploy Azure Cosmos DB MongoDB Cluster monitoring
## This terraform script will deploy the following monitoring alerts for a Cosmos DB MongoDB Cluster

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**  
***The alert priority level is 2***  

2. Committed Memory high  
Whenever the average Committed Memory percent is greater than 90%.  
**This indicates that the system's memory resources are approaching high utilization, potentially impacting performance and responsiveness.**  
***The alert priority level is 3***  

2. Committed Memory critical  
Whenever the average Committed Memory percent is greater than 98%.  
**This signifies a critical situation where the system's memory resources are severely strained, likely leading to performance degradation and potential system instability.**  
***The alert priority level is 2***  

3. CPU Percent high  
Whenever the average CPU* percent is greater than 90%.  
**This alerts to instances where the CPU resources are approaching high utilization, potentially impacting the system's ability to handle processing demands efficiently.**  
***The alert priority level is 3***  

3. CPU Percent critical  
Whenever the average CPU* percent is greater than 98%.  
**This signals a critical situation where the CPU resources are severely strained, likely leading to performance degradation and potential system unresponsiveness.**  
***The alert priority level is 2***  

4. Storage Percent over 80%  
Whenever the average storage percent is greater than 80%.  
**This indicates that the storage resources are approaching high utilization, potentially impacting data availability and system performance.**  
***The alert priority level is 5***  

5. Storage Percent over 90%  
Whenever the average storage percent is greater than 90%.  
**This alerts to situations where the storage resources are reaching a critical level of utilization, potentially leading to data access issues and system instability.**  
***The alert priority level is 4***  

6. Storage Percent over 95%  
Whenever the average storage percent is greater than 95%.  
**This signifies a critical situation where the storage resources are severely strained, potentially leading to data loss or system failures if not addressed promptly.**  
***The alert priority level is 2***  

   > *CPU stands for Central Processing Unit. It is often referred to as the "brain" of the computer because it performs most of the processing inside a computer.  
