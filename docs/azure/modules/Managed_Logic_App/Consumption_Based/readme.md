# Deploy Azure Logic App monitoring
## This terraform script will deploy the following monitoring alerts for a Logic App

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**  
***The alert priority level is 2***  

2. Logic Run Failure Percentage  
Triggered when the total Runs Failed is greater than 0.  
**This indicates the proportion of failed executions of a logic app's workflow, potentially signaling issues with data processing or integration tasks.**  
***The alert priority Level is 3***  

3. Run Latency Medium  
Whenever the average Run Latency is greater than dynamic criteria (Medium)  
**This indicates moderate delay in the execution of a logic app's workflow, potentially affecting its responsiveness or performance.**  
***The alert priority Level is 3***  

4. Run Latency High  
Whenever the average Run Latency is greater than dynamic criteria (Low)  
**This indicates a significant delay in the execution of a logic app's workflow, potentially impacting its responsiveness or causing performance issues.**  
***The alert priority Level is 3***  


