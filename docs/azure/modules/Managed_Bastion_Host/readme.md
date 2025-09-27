# Deploy Azure Bastion Host monitoring
## This terraform script will deploy the following monitoring alerts for a Azure Bastion Network

1. Bastion Communication Status  
Bastion Health status is 0.  
**This indicates communication issues with the bastion network.**  
***The alert priority level is 2***  

2. CPU Usage  
CPU utilization average is higher than 85% utilization.  
**This alert is to prevent CPU throttle and proactive response to increase capacity.**  
***The alert priority level is 3***  

3. Memory Usage  
Memory utilization average is higher than 85% utilization.  
**This alert is to prevent Memory throttle and proactive response to increase capacity.**  
***The alert priority level is 3***  
