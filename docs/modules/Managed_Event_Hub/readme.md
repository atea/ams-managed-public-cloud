# Deploy Azure Event Hub monitoring
This terraform script will deploy the following monitoring alerts for a Event Hub

1. Resource Health  
Resource Health status is no longer 'Available'

2. Event Hub Incoming messages  
Whenever the total Incoming Messages is less than or equal to 0

3. Event Hub Throttled Requests  
Whenever the total Throttled Requests. is greater than 0

4. Event Hub Server Errors  
Whenever the total Server Errors. is greater than 0

5. Event Hub Quota Exceeded Errors  
Whenever the total Quota Exceeded Errors. is greater than 0

6. Event Hub User Errors  
Whenever the total User Errors. is greater than 0





