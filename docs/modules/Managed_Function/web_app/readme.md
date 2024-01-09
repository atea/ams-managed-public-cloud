# Deploy Azure Function App monitoring
This terraform script will deploy the following monitoring alerts for a Function App

1. Resource Health
Resource Health status is no longer 'Available'

2. Http Server Errors  
Whenever the total Http Server Errors is greater than 1

3. Health Check Status  
Whenever the average Health check status is less than 100

4. Response Time Medium  
Whenever the average Response Time is greater than dynamic criteria (Medium)

5. Response Time High  
Whenever the average Response Time is greater than dynamic criteria (High)

6. 4xx error  
Whenever the total Http 4xx is greater than 10



