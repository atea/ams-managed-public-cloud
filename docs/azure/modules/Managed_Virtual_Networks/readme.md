# Deploy Azure Virtual Network monitoring
## This terraform script will deploy the following monitoring alerts for Virtual Networks

1. If Under DDoS Attack  
Whenever the maximum IfUnderDDoSAttack status is greater than 0.  
**This indicates potential DDOS Attack on the network which can affect functionality on all services connected to this network.**  
***The alert priority level is 2***  

2. Activity Log Subnet Write  
Activity Log alert when subnet write succeeds (operation: Microsoft.Network/virtualNetworks/subnets/write).  
**This tracks and verifies subnet configuration changes.**  
***The alert priority level is 4***  
