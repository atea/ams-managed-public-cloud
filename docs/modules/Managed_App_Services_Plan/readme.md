# Deploy Azure App Services Plan monitoring
This terraform script will deploy the following monitoring alerts for App Services Plan

1. Resource Health  
Resource Health status is no longer 'Available'

1. App Services Plan Cpu Percentage High   
Whenever the average CPU Percentage is greater than 90%

1. App Services Plan Cpu Percentage Critical  
Whenever the average CPU Percentage is greater than 98%

1. App Services Plan Memory Percentage High  
Whenever the average memory Percentage is greater than 90%

1. App Services Plan Memory Percentage Critical  
Whenever the average memory Percentage is greater than 98%

1. App Services Plan Http Queue Length  
Whenever the average Http Queue Length is greater than 100




