# Deploy Azure Analysis Services monitoring  
## This terraform script will deploy the following monitoring alerts for a Analysis Services  

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**    
***The alert priority level is 2***  

2. Memory Usage Medium  
Whenever the average Memory Usage is greater than dynamic criteria (Medium).   
**This signifies that system resources are approaching a moderate level of utilization, potentially affecting performance and responsiveness.**   
***The alert priority level is 5***  

3. Memory Usage High  
Whenever the average Memory Usage is greater than dynamic criteria (Low).  
**This highlights a critical situation where system memory resources are under high demand, posing a risk of performance degradation or application failures.**  
***The alert priority level is 4***  

4. QPU Medium  
Whenever the average QPU* is greater than dynamic criteria (Medium).  
**This indicates a moderate load on the system's processing unit, possibly affecting processing speed and overall system responsiveness.**  
***The alert priority level is 5***  

5. QPU High  
Whenever the average QPU* is greater than dynamic criteria (Low).  
**This alerts to a situation where the system's processing unit is under heavy load, potentially causing delays in processing tasks and impacting system performance.**  
***The alert priority level is 4***  

    > *Azure Query Processing Unit (QPU) is a measure of the computing power dedicated to processing database queries efficiently within the Azure cloud environment  







