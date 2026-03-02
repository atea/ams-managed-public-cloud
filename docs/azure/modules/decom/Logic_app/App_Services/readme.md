# Deploy Azure Logic App Services monitoring  
## This terraform script will deploy the following monitoring alerts for a Logic App  

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**    
***The alert priority level is 2***  

2. Health Check Status  
Whenever the average Health check status is less than 100.  
**This indicates potential issues with system health, requiring attention to ensure optimal performance and reliability.**   
***The alert priority level is 2***  

3. Response Time Medium  
Whenever the average Response Time is greater than dynamic criteria (Medium).  
**This alerts to instances where system response times are approaching a moderate level, potentially impacting user experience and operational efficiency.**  
***The alert priority level is 3***  

4. Response Time High  
Whenever the average Response Time is greater than dynamic criteria (Low).  
**This signals critical situations where system response times have reached a high level, potentially causing delays in service delivery and customer dissatisfaction.**  
***The alert priority level is 2***  

5. Workflow Run Failure Rate    
Whenever the total Workflow Runs Failure Rate is greater than 0%.  
**This identifies instances where workflows have encountered failures during execution, indicating potential disruptions in business processes and workflows that need immediate investigation and resolution.**  
***The alert priority level is 3***  





