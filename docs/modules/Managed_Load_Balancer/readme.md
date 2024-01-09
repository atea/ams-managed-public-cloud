# Deploy Azure Load Balancer monitoring
This terraform script will deploy the following monitoring alerts for a Load Balancer

1. Resource Health  
Resource Health status is no longer 'Available'

2. Load Balancer Health Probe Status  
Whenever the average Health Probe Status is less than 100

3. Load Balancer Used SNAT Ports  
Whenever the average Used SNAT Ports is greater than 900

4. Load Balancer Data Path Availability  
Whenever the average Data Path Availability is less than 100

