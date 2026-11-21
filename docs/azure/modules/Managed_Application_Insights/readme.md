# Deploy Azure Application Insights monitoring
## This terraform script will deploy the following monitoring alerts for a Application Insights

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**  
***The alert priority level is 2***  

2. Availability   
Whenever the average Availability is less than 100%.  
**This indicates potential issues with the availability of the system or service, which may impact user access and reliability.**  
***The alert priority level is 2***  

3. Failed requests  
Whenever the count Failed requests is greater than 0.  
**This alerts to instances where requests to the system or service have failed, potentially indicating issues with functionality or connectivity.**  
***The alert priority level is 3***  

4. Exceptions   
Whenever the count Exceptions is greater than 0.  
**This indicates instances where the system or service has encountered errors or unexpected conditions, potentially affecting its operation and reliability.**  
***The alert priority level is 5***  

5. Server response time High  
Whenever the average Server response time is greater than dynamic criteria (High).  
**This signals critical situations where the server response time has reached a high level, potentially causing delays in service delivery and customer dissatisfaction.**  
***The alert priority level is 3***  

6. Server exceptions    
Whenever the count Server exceptions is greater than 5.  
**This indicates instances where the server has encountered multiple exceptions, potentially indicating systemic issues or instability.**  
***The alert priority level is 4***  





