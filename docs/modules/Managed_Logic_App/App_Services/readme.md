# Deploy Azure Logic App monitoring
This terraform script will deploy the following monitoring alerts for a Logic App

1. Resource Health  
Resource Health status is no longer 'Available'

2. Health Check Status  
Whenever the average Health check status is less than 100

3. Response Time Medium  
Whenever the average Response Time is greater than dynamic criteria (Medium)

4. Response Time High  
Whenever the average Response Time is greater than dynamic criteria (High)

5. Workflow Run Failure Rate  
Whenever the total Workflow Runs Failure Rate is greater than 0%