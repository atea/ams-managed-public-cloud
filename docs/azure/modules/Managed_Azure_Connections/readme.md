# Deploy Azure Network Ingressing and Egressing monitoring
## This terraform script will deploy the following monitoring alerts for Azure Network connections

1. Bits In Per Second  
Whenever the average Bits ingressing Azure per second is greater than 6,000,000,000 bps (6 Gbps).  
**This indicates potential unexpected data traffic to your Azure network.**  
***The alert priority level is 4***  

2. Bits Out Per Second  
Whenever the average Bits egressing Azure per second is greater than 6,000,000,000 bps (6 Gbps).  
**This indicates potential unexpected data traffic from your Azure network.**  
***The alert priority level is 4***  
