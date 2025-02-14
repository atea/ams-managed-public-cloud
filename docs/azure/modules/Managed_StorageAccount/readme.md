# Deploy Azure Storage Account monitoring
## This terraform script will deploy the following monitoring alerts for a Storage Account

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**  
***The alert priority level is 2***  

2. Availability  
The Storage Account is no longer available, please investigate.  
**This indicates a decrease in the availability of the service or resource, potentially impacting users' ability to access and utilize it.**  
***The alert priority Level is 2***  

3. Egress  
Whenever the total Egress is greater than dynamic threshold.  
**This indicates high outbound data transfer from the service or resource, potentially leading to increased costs or impacting network performance.**  
***The alert priority Level is 5***  

4. Ingress  
Whenever the total Ingress is greater than dynamic threshold.  
**This indicates high inbound data transfer to the service or resource, potentially impacting network performance or indicating increased usage.**  
***The alert priority Level is 5***  

5. Blob Transactions  
Whenever the blob transactions is greater than dynamic threshold.  
**This indicates high activity on Blob storage, potentially impacting performance or indicating increased usage.**  
***The alert priority Level is 5***  

6. Success Server Latency  
The Storage Account Success Server Latency is more than 1000ms average over 5 minutes.  
**This indicates delayed response times for successful requests from the server, potentially impacting user experience or indicating performance issues.**  
***The alert priority Level is 2***  