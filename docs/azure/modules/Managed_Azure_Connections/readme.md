# Deploy Azure Network Ingressing and Egressing monitoring
## This terraform script will deploy the following monitoring alerts for a Azure Network connections

1. Bits In Per Second  
Bits ingressing Azure per second greater than [X].  
**This indicates potential unexpected data traffic to your Azure network.**  
***The alert priority level is 4***  

2. Bits Out Per Second  
Bits egressing Azure per second greater than [X].  
**This indicates potential unexpected data traffic from your Azure network.**  
***The alert priority level is 4***  
