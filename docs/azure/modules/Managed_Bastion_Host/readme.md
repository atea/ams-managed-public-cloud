# Deploy Azure Bastion Host monitoring
## This terraform script will deploy the following monitoring alerts for a Azure Bastion Network

1. CPU Usage  
Whenever the average CPU utilization (usage_user) is greater than 85%.  
**This alert is to prevent CPU throttle and proactive response to increase capacity.**  
***The alert priority level is 4***  

2. Memory Usage  
Whenever the average Memory utilization (used) is greater than 85%.  
**This alert is to prevent Memory throttle and proactive response to increase capacity.**  
***The alert priority level is 4***  

3. Bastion Communication Status  
Whenever the average pingmesh is less than 1.  
**This indicates communication issues with the bastion network.**  
***The alert priority level is 3***  
