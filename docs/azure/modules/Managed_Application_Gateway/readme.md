# Deploy Azure Application Gateway monitoring
## This terraform script will deploy the following monitoring alerts for a Application Gateway

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**  
***The alert priority level is 2***  

2. Application Gateway Unhealthy Host Count  
Whenever the average Unhealthy Host Count is greater than 0.  
**This indicates potential issues with the health or availability of backend hosts, which may impact the overall performance and reliability of the application.**  
***The alert priority level is 3***  

3. Application Gateway Failed requests  
Whenever the total Failed Requests is greater than 10.  
**This alerts to instances where requests to the application gateway have failed, potentially indicating issues with connectivity, configuration, or backend services.**  
***The alert priority level is 3***  

4. Application Gateway healthy host count  
Whenever the average Healthy Host Count is less than 1.  
**This indicates situations where all backend hosts are deemed unhealthy, potentially causing service disruptions and requiring immediate attention.**  
***The alert priority level is 3***  

5. Application Gateway Total time  
Whenever the average Application Gateway Total Time is greater or less than dynamic criteria.  
**This measures the overall performance of the application gateway in processing requests, with deviations from expected values potentially indicating issues with latency or processing efficiency.**  
***The alert priority level is 3***  




