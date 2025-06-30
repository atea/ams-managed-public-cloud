# Deploy Azure IoT Hub monitoring
## This terraform script will deploy the following monitoring alerts for a IoT Hub

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**    
***The alert priority level is 2***  

2. IoT Hub Total Number of Messages Used  
Whenever the maximum Total number of messages used is greater than dynamic criteria.  
**This refers to the aggregate count of messages that have been processed or transmitted through an Azure IoT Hub within a specific timeframe.**  
***The alert priority Level is 5***  

3. Total Number of Devices  
Whenever the average Connected devices is greater than or equal to 5.  
**This typically refers to the cumulative count of all devices that are registered or connected to a specific platform, service, or system. In the context of IoT, it represents the overall quantity of physical devices or endpoints that are actively communicating with an IoT platform, such as Azure IoT Hub.**  
***The alert priority Level is 5***

4. IoT Hub Total Number Throttling errors  
Whenever the total Number of throttling errors is greater than 0.  
**refers to the aggregate count of instances where requests or operations made to an Azure IoT Hub have been throttled or limited due to exceeding usage quotas or service limits within a specified time period.**  
***The alert priority Level is 3***

5. IoT Hub Total Number of Messages Used  
Whenever the total Telemetry messages sent is greater than dynamic criteria.  
**This refers to the cumulative count of telemetry messages transmitted through an Azure IoT Hub within a specified time frame.**  
***The alert priority Level is 5***  

6. IoT Hub Total Routing telemetry messages dropped  
Whenever the total Routing telemetry messages dropped is greater than 0.  
**This refers to the cumulative count of telemetry messages that were intended for routing within an Azure IoT Hub but were ultimately discarded or dropped without being successfully processed or delivered to their intended destinations.**  
***The alert priority Level is 3***  





