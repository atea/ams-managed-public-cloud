# Deploy Azure IoT Hub monitoring
This terraform script will deploy the following monitoring alerts for a IoT Hub

1. Resource Health  
Resource Health status is no longer 'Available'

2. IoT Hub Total Number of Messages Used  
Whenever the maximum Total number of messages used is greater or less than dynamic criteria

3. Total Number of Devices  
Whenever the average Connected devices is greater than or equal to 5

4. IoT Hub Total Number Throttling errors  
Whenever the total Number of throttling errors is greater than 0

5. IoT Hub Total Number of Messages Used  
Whenever the total Telemetry messages sent is greater or less than dynamic criteria

6. IoT Hub Total Routing telemetry messages dropped
Whenever the total Routing telemetry messages dropped is greater than 0





