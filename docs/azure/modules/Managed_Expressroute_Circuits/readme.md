# Deploy Azure Express route circuits monitoring
## This terraform script will deploy the following monitoring alerts for Express route circuits

1. ARP Availability  
ARP Availability from MSEE towards all peers is less than 90%.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**  
***The alert priority level is 1***  

2. BGP Availability  
BGP Availability from MSEE towards all peers is less than 90%.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**  
***The alert priority level is 1***  

3. Bits In Per Second  
Bits ingressing Azure expressroute circuits per second greater than [X].  
**This indicates potential unexpected data traffic to your Azure network through the express route.**  
***The alert priority level is 3***  

4. Bits Out Per Second  
Bits egressing Azure expressroute circuits per second greater than [X].  
**This indicates potential unexpected data traffic from your Azure network through the express route.**  
***The alert priority level is 3***  

5. Global reach bits in per second  
Bits ingressing Azure expressroute circuits global reach per second greater than [X].  
**This indicates potential unexpected data traffic to your Azure network through the express route.**  
***The alert priority level is 3***  

6. Global reach bits out per second  
Bits egressing Azure expressroute circuits global reach per second greater than [X].  
**This indicates potential unexpected data traffic from your Azure network through the express route.**  
***The alert priority level is 3***  

7. Qos Drop Bits In Per Second  
Compute Unit utilization crosses 75% of average usage.  
**This indicates potential issues with the data traffic to your Azure network through the express route.**  
***The alert priority level is 3***  

8. Qos Drop Bits Out Per Second  
Bits egressing dropped for Azure expressroute circuits per second greater than [X] (dynamic).  
**This indicates potential issues with the data traffic from your Azure network through the express route.**  
***The alert priority level is 3***  
