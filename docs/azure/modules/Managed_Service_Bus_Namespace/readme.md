# Deploy Azure Service Bus Namespace monitoring
## This terraform script will deploy the following monitoring alerts for a Service Bus Namespace

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**    
***The alert priority level is 2***  

2. Dead-Lettered Messages  
Whenever the average count of dead-lettered messages in a Queue/Topic is greater than 2  
**This indicates messages that failed processing multiple times and were moved to a dead-letter queue for further analysis, potentially indicating issues with message processing or system errors.**  
***The alert priority Level is 5***  




