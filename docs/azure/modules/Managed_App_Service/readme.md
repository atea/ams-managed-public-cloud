# Deploy Azure App Service monitoring
## This terraform script will deploy the following monitoring alerts for a App Service

1. Health Check Status  
Whenever the average Health check status is less than 100.  
**This indicates potential issues with system health, requiring attention to ensure optimal performance and reliability.**  
***The alert priority level is 3***  

2. Response Time High  
Whenever the average Response Time is greater than dynamic criteria (Low).  
**This signals critical situations where system response times have reached a high level, potentially causing delays in service delivery and customer dissatisfaction.**  
***The alert priority level is 2***  

3. Http Server Errors Medium  
Whenever the total Http Server Errors* is greater than dynamic criteria (Medium).  
**This indicates instances where the server encounters a moderate level of errors in handling client requests, potentially impacting user experience and service reliability.**
***The alert priority level is 4***  

4. Http Server Errors High  
Whenever the total Http Server Errors* is greater than dynamic criteria (Low).  
**This alerts to critical situations where the server experiences a high number of errors in handling client requests, potentially causing service disruptions and requiring immediate attention.**  
***The alert priority level is 3***  

5. 4xx error Medium  
Whenever the total Http4xx** is greater than dynamic criteria (Medium).  
**This indicates instances where the server encounters a moderate level of client request errors, potentially indicating issues with user input or system configuration.**  
***The alert priority level is 4***  

6. 4xx error High  
Whenever the total Http4xx** is greater than dynamic criteria (Low).  
**This alerts to critical situations where the server experiences a high number of client request errors, potentially indicating systemic issues or security vulnerabilities.**  
***The alert priority level is 2***  

7. Logic App Workflow Run Failure Rate (Logic Apps on app services plan)  
Whenever the total Workflow Runs Failure Rate is greater than 0%.  
**This indicates instances where there are failures in the execution of logic app workflows, potentially disrupting business processes and requiring investigation and resolution.**
***The alert priority level is 3***  

    > *HTTP Server Errors refer to errors encountered on the server side while processing client requests.    
    > **HTTP 4xx errors refer to client error responses from the server. These errors indicate that the client's request cannot be fulfilled due to issues such as invalid syntax, unauthorized access, or resource not found.   
