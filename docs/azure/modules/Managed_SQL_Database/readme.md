# Deploy Azure SQL Database monitoring
## This terraform script will deploy the following monitoring alerts for a SQL Database

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**    
***The alert priority level is 2***  

2. SQL Database Data Space Used Percent over 80%  
Whenever the maximum Data space used percent is greater than 80%.  
**This indicates that the data space allocated for the SQL database is reaching a high utilization level, potentially impacting performance and requiring attention to manage storage capacity.**  
***The alert priority Level is 5***  

3. SQL Database Data Space Used Percent over 90%  
Whenever the maximum Data space used percent is greater than 90%.  
**This indicates that the data space allocated for the SQL database is critically high, potentially leading to performance degradation and requiring immediate action to manage storage capacity.**  
***The alert priority Level is 2***  

4. SQL Database Data Space Used Percent over 95%  
Whenever the maximum Data space used percent is greater than 95%.  
**This indicates an urgent situation where the data space allocated for the SQL database is severely high, risking performance degradation and requiring immediate action to prevent service disruptions and potential data loss.**  
***The alert priority Level is 2***  

5. SQL Database CPU Percent high  
Whenever the average CPU percentage is greater than 90%.  
**This indicates high CPU utilization within the SQL database, potentially impacting performance and responsiveness of database operations.**  
***The alert priority Level is 3***  

6. SQL Database CPU Percent critical  
Whenever the average CPU percentage is greater than 98%.  
**This indicates an urgent situation where the CPU usage of the SQL database is critically high, causing severe performance degradation and requiring immediate action to prevent service outages.**  
***The alert priority Level is 2***

7. SQL Database Workers Percent high  
Whenever the average Workers percentage is greater than 90%.  
**This indicates high utilization of workers within the SQL database, potentially impacting its ability to handle concurrent requests and affecting overall performance.**  
***The alert priority Level is 3***  

8. SQL Database Workers Percent critical  
Whenever the average Workers percentage is greater than 90%.
**This indicates an urgent situation where the SQL database is overwhelmed with concurrent requests, causing severe performance degradation and requiring immediate action to prevent service outages.**  
***The alert priority Level is 2***  

9. SQL Database Failed Connections  
Whenever the total Failed Connections : System Errors is greater than 1.
**This indicates issues with establishing connections to the SQL database, potentially impacting application functionality and requiring investigation to identify and resolve connectivity issues.**  
***The alert priority Level is 3***  

10. SQL Database Deadlock  
Whenever the total Deadlocks is greater than 1.  
**This indicates a situation where two or more transactions are waiting for each other to release locks, potentially causing performance degradation and requiring investigation to resolve concurrency issues.**  
***The alert priority Level is 4***  

11. SQL DTU over 90 percent  
Whenever the average DTU usage is over 90% over 30 minutes.  
**This indicates high resource utilization within the SQL Database, potentially impacting performance and responsiveness of database operations.**  
***The alert priority Level is 3***  

12. SQL DTU 100 percent  
Whenever the average DTU usage is 100% for 15 minutes.  
**This indicates maximum resource utilization within the SQL Database, potentially causing severe performance degradation and requiring immediate action to prevent service disruptions.**  
***The alert priority Level is 2***  

13. SQL Data IO percentage high  
Whenever the average Data IO percentage is greater than 90%.  
**This alert signifies instances where the data input-output (IO) operations are approaching high utilization, potentially impacting system performance and responsiveness. Addressing these events promptly ensures smooth data processing and maintains operational efficiency.**  
***The alert priority Level is 3***  

14. SQL Data IO percentage critical  
Whenever the average Data IO percentage is greater than 98%.  
**This alert signifies instances where the data input-output (IO) operations are approaching high utilization, potentially impacting system performance and responsiveness. Addressing these events promptly ensures smooth data processing and maintains operational efficiency.**  
***The alert priority Level is 2***  