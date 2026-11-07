# Deploy Azure Data Factory monitoring
## This terraform script will deploy the following monitoring alerts for a Data Factory

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**  
***The alert priority level is 2***  

2. Data Factory Failed Pipeline runs metrics  
Whenever the total Failed pipeline runs metrics is greater than 0.  
**This indicates instances where data processing pipelines have encountered failures, potentially leading to data inconsistencies or disruptions in data workflows.**  
***The alert priority level is 3***    




