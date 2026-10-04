# Deploy Azure Application Gateway monitoring
## This terraform script will deploy the following monitoring alerts for an Application Gateway

1. Application Gateway Total Time  
Whenever the average Application Gateway Total Time is greater or less than dynamic criteria (Medium sensitivity).  
**This measures the overall performance of the application gateway in processing requests, with deviations from expected values potentially indicating issues with latency or processing efficiency.**  
***The alert priority level is 3***  

2. Failed Requests  
Whenever the total Failed Requests is greater than 10.  
**This alert to instances where requests to the application gateway have failed, potentially indicating issues with connectivity, configuration, or backend services.**  
***The alert priority level is 3***  

3. Healthy Host Count  
Whenever the average Healthy Host Count is less than 1.  
**This indicates situations where all backend hosts are deemed unhealthy, potentially causing service disruptions and requiring immediate attention.**  
***The alert priority level is 3***  

4. Unhealthy Host Count  
Whenever the average Unhealthy Host Count is greater than 0.  
**This indicates potential issues with the health or availability of backend hosts, which may impact the overall performance and reliability of the application.**  
***The alert priority level is 3***
