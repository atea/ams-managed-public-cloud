# Deploy Azure Event Hub monitoring  
## This terraform script will deploy the following monitoring alerts for a Analysis Services  

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**    
***The alert priority level is 2***  

2. Event Hub Incoming messages  
Whenever the total Incoming Messages is less than or equal to 0.  
**This refers to the data or events being sent to an Azure Event Hub from various sources such as applications or devices for real-time processing and storage within the Event Hub service.**  
***The alert priority level is 3***

3. Event Hub Throttled Requests  
Whenever the total Throttled Requests. is greater than 0.  
**This indicates that the Event Hub service is currently enforcing rate limits on incoming data requests to prevent overload and maintain optimal performance and stability.**  
***The alert priority level is 3***  

4. Event Hub Server Errors  
Whenever the total Server Errors. is greater than 0.  
**This refer to issues or problems encountered on the server side of an Azure Event Hub service.**  
***The alert priority level is 2***  

5. Event Hub Quota Exceeded Errors  
Whenever the total Quota Exceeded Errors. is greater than 0.  
**This occur when the usage of an Azure Event Hub service exceeds the allocated quota or limit for certain resources**  
***The alert priority Level is 4***  

6. Event Hub User Errors  
Whenever the total User Errors. is greater than 0.  
**This typically refer to mistakes or issues originating from the user's side when interacting with an Azure Event Hub service.**  
***The alert priority Level is 3***  





