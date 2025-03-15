# Deploy Azure Cosmos DB PostgreSQL monitoring
## This terraform script will deploy the following monitoring alerts for a Cosmos DB PostgreSQL

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**  
***The alert priority level is 2***  

2. CPU Percent high  
Whenever the average CPU* percent is greater than 90%.  
**This indicates that the CPU resources are approaching high utilization, potentially impacting system performance and responsiveness.**  
***The alert priority level is 3***  

2. CPU Percent critical  
Whenever the average CPU* percent is greater than 90%.  
**This signals a critical situation where the CPU resources are severely strained, likely leading to performance degradation and potential system instability.**  
***The alert priority level is 2***  

3. Memory Percent high  
Whenever the average Memory percent is greater than 90%.  
**This alerts to instances where the memory resources are approaching high utilization, potentially impacting system stability and causing slowdowns.**  
***The alert priority level is 3***  

3. Memory Percent critical  
Whenever the average Memory percent is greater than 90%.  
**This signifies a critical situation where the memory resources are severely strained, likely leading to performance degradation and potential system crashes.**  
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

7. IOPS Consumed Percentage  High
Whenever the average VM Cached IOPS Consumed Percentage is greater than 90%.  
**This indicates that the Input/Output Operations Per Second (IOPS) consumed by the virtual machine's cache are approaching high utilization, potentially impacting disk performance and responsiveness.**  
***The alert priority level is 3***  

8. IOPS Consumed Percentage Critical
Whenever the average VM Cached IOPS Consumed Percentage is greater than 98%.  
**This signifies a critical situation where the Input/Output Operations Per Second (IOPS) consumed by the virtual machine's cache are severely strained, potentially leading to significant degradation in disk performance and responsiveness. Immediate attention is required to prevent system instability and potential data loss.**  
***The alert priority level is 3***  

   > *CPU stands for Central Processing Unit. It is often referred to as the "brain" of the computer because it performs most of the processing inside a computer.  
   > **IOPS (Input/Output Operations Per Second) refers to the measure of the number of read and write operations that occur to a storage resource, such as Azure Managed Disks or Azure Blob Storage, in one second.




