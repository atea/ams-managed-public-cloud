# Deploy Azure Stream Analytics Job monitoring with Terraform 
This terraform script will deploy the following monitoring alerts for a Stream Analytics Job

1. Resource Health  
Resource Health status is no longer 'Available'

2. Watermark Delay   
Whenever the maximum Watermarc Delay is greater or less than dynamic criteria

3. Memory utilization over 90%  
Whenever the maximum SU(Memory)% Utilization is greater than 90%

4. Memory utilization over 98%  
Whenever the maximum SU(Memory)% Utilization is greater or equal than 98%

5. Runtime Errors  
Whenever the total Runtime Errors(Sum) is greater than 0

6. Data Conversation Errors  
Whenever the total Data Conversation Errors(Sum) is greater than 0







