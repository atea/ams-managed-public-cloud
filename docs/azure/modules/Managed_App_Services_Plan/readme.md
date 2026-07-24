# Deploy Azure App Services Plan monitoring
## This terraform script will deploy the following monitoring alerts for App Services Plan

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**  
***The alert priority level is 2***  

1. App Services Plan CPU Percentage High   
Whenever the average CPU* Percentage is greater than 90%.  
**This indicates that the CPU resources allocated to the app service plan are nearing their maximum capacity, potentially impacting the performance and responsiveness of hosted applications.**  
***The alert priority level is 4***  

1. App Services Plan CPU Percentage Critical  
Whenever the average CPU* Percentage is greater than 98%.  
**This signifies a critical situation where the CPU resources allocated to the app service plan are severely strained, likely leading to performance degradation and service interruptions.**  
***The alert priority level is 2***  

1. App Services Plan Memory Percentage High  
Whenever the average memory Percentage is greater than 90%.  
**This indicates that the memory resources allocated to the app service plan are approaching their maximum capacity, potentially impacting the stability and availability of hosted applications.**  
***The alert priority level is 4***  

1. App Services Plan Memory Percentage Critical  
Whenever the average memory Percentage is greater than 98%.  
**This alerts to a critical situation where the memory resources allocated to the app service plan are severely strained, likely leading to performance degradation and potential service disruptions.**  
***The alert priority level is 2***  

1. App Services Plan Http Queue Length**  
Whenever the average Http Queue Length is greater than 100.  
**This indicates a backlog of HTTP requests waiting to be processed by the app service plan, potentially causing delays in request handling and impacting the overall responsiveness of hosted applications.**  
***The alert priority level is 3***  

   > *CPU stands for Central Processing Unit. It is often referred to as the "brain" of the computer because it performs most of the processing inside a computer.  
   > **HTTP Queue Length refers to the number of HTTP requests waiting in the queue to be processed by the server. When the server receives more requests than it can handle immediately, the excess requests are placed in a queue to be processed in order.  