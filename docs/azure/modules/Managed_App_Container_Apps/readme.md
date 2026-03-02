# Deploy Azure Container Apps monitoring
## This terraform script will deploy the following monitoring alerts for Container Apps

1. Container Apps CPU Percentage High   
Whenever the average CPU Percentage is greater than 90%.  
**This indicates that the CPU resources allocated to the container app are nearing their maximum capacity, potentially impacting the performance and responsiveness of hosted applications.**  
***The alert priority level is 4***  

1. Container Apps CPU Percentage Critical  
Whenever the average CPU Percentage is greater than 98%.  
**This signifies a critical situation where the CPU resources allocated to the container app are severely strained, likely leading to performance degradation and service interruptions.**  
***The alert priority level is 2***  