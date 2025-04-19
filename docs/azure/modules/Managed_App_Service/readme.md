# Deploy Azure App Service monitoring
## This terraform script will deploy the following monitoring alerts for a App Service

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**  
***The alert priority level is 2*** 

2. Health Check Status  
Whenever the average Health check status is less than 100.  
**This indicates potential issues with system health, requiring attention to ensure optimal performance and reliability.**  
***The alert priority level is 3***  

3. Response Time Medium  
Whenever the average Response Time is greater than dynamic criteria (Medium).  
**This alerts to instances where system response times are approaching a moderate level, potentially impacting user experience and operational efficiency.**  
***The alert priority level is 3***  

4. Response Time High  
Whenever the average Response Time is greater than dynamic criteria (Low).  
**This signals critical situations where system response times have reached a high level, potentially causing delays in service delivery and customer dissatisfaction.**  
***The alert priority level is 2***  

5. Http Server Errors Medium  
Whenever the total Http Server Errors* is greater than dynamic criteria (Medium).  
**This indicates instances where the server encounters a moderate level of errors in handling client requests, potentially impacting user experience and service reliability.**
***The alert priority level is 4***  

6. Http Server Errors High  
Whenever the total Http Server Errors* is greater than dynamic criteria (Low).  
**This alerts to critical situations where the server experiences a high number of errors in handling client requests, potentially causing service disruptions and requiring immediate attention.**  
***The alert priority level is 3***  

7. 4xx error Medium  
Whenever the total Http4xx** is greater than dynamic criteria (Medium).  
**This indicates instances where the server encounters a moderate level of client request errors, potentially indicating issues with user input or system configuration.**  
***The alert priority level is 4***  

8. 4xx error High  
Whenever the total Http4xx** is greater than dynamic criteria (Low).  
**This alerts to critical situations where the server experiences a high number of client request errors, potentially indicating systemic issues or security vulnerabilities.**  
***The alert priority level is 2***  

9. Logic App Workflow Run Failure Rate (Logic Apps on app services plan)  
Whenever the total Workflow Runs Failure Rate is greater than 0%.  
**This indicates instances where there are failures in the execution of logic app workflows, potentially disrupting business processes and requiring investigation and resolution.**
***The alert priority level is 3***  

    > *HTTP Server Errors refer to errors encountered on the server side while processing client requests.    
    > **HTTP 4xx errors refer to client error responses from the server. These errors indicate that the client's request cannot be fulfilled due to issues such as invalid syntax, unauthorized access, or resource not found.   
