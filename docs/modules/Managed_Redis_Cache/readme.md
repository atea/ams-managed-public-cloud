# Deploy Azure Cache for Redis monitoring
This terraform script will deploy the following monitoring alerts for a Cache for Redis

1. Resource Health  
Resource Health status is no longer 'Available'

2. Server Load High  
Whenever the average Server Load is greater than 90%

3. Server Load Critical  
Whenever the average Server Load is greater than 98%

4. Used Memory  
Whenever the average Used Memory Percentage is greater than 90%

5. Used Memory Critical  
Whenever the average Used Memory Percentage is greater than 98%

6. Connected Clients  
Whenever the maximum Connected Clients is greater than 5625

7. Cache Read  
Whenever the maximum Cache Read is greater or less than dynamic criteria

8. CPU
Whenever the maximum CPU is greater than 90%

9. CPU Critical
Whenever the maximum CPU is greater than 98%





