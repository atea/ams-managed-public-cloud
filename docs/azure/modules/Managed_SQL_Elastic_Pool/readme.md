# Deploy Azure SQL Elastic Pool monitoring
## This terraform script will deploy the following monitoring alerts for a SQL Elastic Pool

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**    
***The alert priority level is 2***  

2. Data space used percent proactive  
Whenever the average Data space used percent is greater than 80%.  
**This indicates that the data space allocated for storage is approaching a predetermined proactive threshold, prompting proactive capacity planning measures to ensure optimal storage management and prevent potential performance issues.**  
***The alert priority Level is 5***  

3. Data space used percent high  
Whenever the average Data space used percent is greater than 90%.  
**This indicates high utilization of data space in the storage system, potentially approaching capacity limits and requiring attention to prevent storage shortages and ensure continued system operation.**  
***The alert priority Level is 2***  

4. Data space used percent critical  
Whenever the average Data space used percent is greater than 95%.  
**This indicates an urgent situation where the data space used in the storage system has reached a critically high level, posing an immediate risk of storage shortages and service outages.**  
***The alert priority Level is 2**  

5. CPU percentage high  
Whenever the average CPU percentage is greater than 90%.  
**This indicates high CPU utilization, potentially impacting system performance and responsiveness.**  
***he alert priority Level is 3***  

6. CPU percentage critical  
Whenever the average CPU percentage is greater than 98%.  
**This indicates an urgent situation where the CPU usage percentage is critically high, causing severe performance degradation and requiring immediate action to prevent service outages.**  
***The alert priority Level is 2***

7. Data space allocated percent proactive  
Whenever the maximum Data space allocated percent is greater than 80%.  
**This indicates that the allocated data space in the storage system is approaching a predetermined proactive threshold.**  
***The alert priority Level is 5***  

8. Data space allocated percent high  
Whenever the maximum Data space allocated percent is greater than 90%.  
**This indicates high utilization of allocated data space in the storage system, potentially approaching capacity limits and requiring attention to prevent storage shortages and ensure continued system operation.**  
***The alert priority Level is 4***  

9. Data space allocated percent critical  
Whenever the maximum Data space allocated percent is greater than 95%.  
**This indicates an urgent situation where the percentage of allocated data space in the storage system has reached a critically high level, posing an immediate risk of storage shortages and service outages. Immediate action is required to mitigate the risk and prevent disruptions.**  
***The alert priority Level is 2***  

10. Data IO percentage High  
Whenever the average Data IO percentage is greater than 90%.  
**This indicates high data input/output (IO) activity, potentially affecting system performance.**  
***The alert priority Level is 3***  

11. Data IO percentage Critical  
Whenever the average Data IO percentage is greater than 98%.  
**This indicates an urgent situation where the percentage of data input/output (IO) activity is critically high.**  
***The alert priority Level is 2***  

12. SQL DTU over 90 percent  
Whenever the average DTU usage is over 90% over 30 minutes.  
**This indicates high resource utilization within the SQL Database, potentially impacting performance and responsiveness of database operations.**  
***The alert priority Level is 2***  

13. SQL DTU 100 percent  
Whenever the average DTU usage is 100% for 15 minutes.  
**This indicates maximum resource utilization within the SQL Database, potentially causing severe performance degradation and requiring immediate action to prevent service disruptions.**  
***The alert priority Level is 2***  



