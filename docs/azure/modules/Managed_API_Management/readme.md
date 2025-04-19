# Deploy Azure API Management monitoring
## This terraform script will deploy the following monitoring alerts for a API Management

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**  
***The alert priority level is 2***  

2. API Management Total Requests  
Whenever the total Requests is greater or less than dynamic criteria.  
**This indicates instances where there's a significant variation in the number of requests, which may affect the performance and usage of the API.***  
***The alert priority level is 3***  

3. Average Capacity High  
Whenever the average Capacity is greater than 90% for 15 minutes.  
**This indicates that the API Management system is operating at a high level of utilization, approaching maximum capacity.**  
***The alert priority level is 3***  

4. Average Capacity Critical  
Whenever the average Capacity is greater than 98% for 15 minutes.  
**This signals a critical situation where the API Management system is severely strained, potentially leading to performance degradation and service interruptions.**  
***The alert priority level is 2***  

5. Duration of Backend Requests  
Whenever the average Duration of Backend Requests is greater than dynamic criteria.  
**This alerts to situations where there's a delay in processing backend requests, impacting the overall responsiveness of the API.**  
***The alert priority level is 3***  

6. Duration of Gateway Requests  
Whenever the average Overall Duration of Gateway Requests is greater than dynamic criteria.   
**This alerts to situations where there's a delay in processing requests at the gateway level, potentially affecting the overall performance and user experience of the API.**  
***The alert priority level is 3***  

    > *API - Application Programming Interface. API acts as a bridge between different software components, allowing them to exchange information and perform specific actions.  


