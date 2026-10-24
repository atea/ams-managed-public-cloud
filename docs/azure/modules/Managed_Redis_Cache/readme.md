# Deploy Azure Cache for Redis monitoring
## This terraform script will deploy the following monitoring alerts for a Cache for Redis

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**  
***The alert priority level is 2***  

2. Server Load High  
Whenever the average Server Load is greater than 90%  
**This indicates a high level of demand on the server's resources, potentially impacting performance and responsiveness.**  
***The alert priority Level is 3***  

3. Server Load Critical  
Whenever the average Server Load is greater than 98%  
**This indicates an urgent situation where the server's resources are overwhelmed, causing severe performance degradation or service outages.**  
***The alert priority Level is 2***  

4. Used Memory  
Whenever the average Used Memory Percentage is greater than 90%  
**This indicates a high level of memory usage on the server, potentially affecting performance and responsiveness.**  
***The alert priority Level is 2***  

5. Used Memory Critical  
Whenever the average Used Memory Percentage is greater than 98%  
**This indicates a high level of memory usage on the server, potentially affecting performance and responsiveness.**  
***The alert priority Level is 2***  

6. Connected Clients  
Whenever the maximum Connected Clients is greater than 5625  
**This indicates a high demand on the service, potentially impacting performance and responsiveness for connected users.**  
***The alert priority Level is 5***  

7. Cache Read  
Whenever the maximum Cache Read is greater than dynamic criteria  
**This indicates frequent access to cached data, which can improve performance by reducing the need to fetch data from the source.**  
***The alert priority Level is 5***  

8. CPU  
Whenever the maximum CPU is greater than 90%  
**This indicates high CPU utilization, potentially impacting system performance and responsiveness.**  
***The alert priority Level is 3***  

9. CPU Critical  
Whenever the maximum CPU is greater than 98%  
**This indicates an urgent situation where the CPU is overwhelmed, causing severe performance degradation or service outages.**  
***The alert priority Level is 2***  





