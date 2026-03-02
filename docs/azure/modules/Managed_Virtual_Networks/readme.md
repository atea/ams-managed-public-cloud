# Deploy Azure Virtual Network monitoring
## This terraform script will deploy the following monitoring alerts for a Virtual Network

1. If Under DDoS Attack  
IfUnderDDoSAttack status is greater than 0.  
**This indicates potential DDOS Attack on the network which can affect functionality on all services connected to this network.**  
***The alert priority level is 2***  
