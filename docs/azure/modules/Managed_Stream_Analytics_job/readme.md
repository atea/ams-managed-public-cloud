# Deploy Azure Stream Analytics Job monitoring with Terraform 
## This terraform script will deploy the following monitoring alerts for a Stream Analytics Job

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**  
***The alert priority level is 2***  

2. Watermark Delay   
Whenever the maximum Watermarc Delay is greater than dynamic criteria.  
**This indicates a delay in processing data beyond a predefined watermark threshold**  
***The alert priority level is 4***  

3. Memory utilization over 90%  
Whenever the maximum SU(Memory)% Utilization is greater than 90%.  
**This indicates high memory usage, potentially impacting system performance and responsiveness due to limited available memory.**  
***The alert priority Level is 2***  

4. Memory utilization over 98%  
Whenever the maximum SU(Memory)% Utilization is greater or equal than 98%.  
**This indicates critically high memory usage, potentially leading to severe performance degradation and system instability due to limited available memory.**  
***The alert priority Level is 2***  

5. Runtime Errors  
Whenever the total Runtime Errors(Sum) is greater than 0.  
**This indicates issues or failures during the execution of code or processes within the system or application.**  
***The alert priority Level is 2***  

6. Data Conversation Errors  
Whenever the total Data Conversation Errors(Sum) is greater than 0.  
**This indicates issues or failures when converting data from one format to another within the system or application**  
***The alert priority Level is 5***  







