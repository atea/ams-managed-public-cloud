# Deploy Azure API Management monitoring
This terraform script will deploy the following monitoring alerts for a API Management

1. Resource Health  
Resource Health status is no longer 'Available'

2. API Management Total Requests  
Whenever the total Requests is greater or less than dynamic criteria

3. Average Capacity high  
Whenever the average Capacity is greater than 90% for 15 minutes

4. Average Capacity Critical  
Whenever the average Capacity is greater than 98% for 15 minutes

5. Duration of Backend Requests  
Whenever the average Duration of Backend Requests is greater than dynamic criteria

6. Duration of Gateway Requests  
Whenever the average Overall Duration of Gateway Requests is greater than dynamic criteria





