# Deploy Azure Express route circuits monitoring
## This terraform script will deploy the following monitoring alerts for Express route circuits

1. ARP Availability  
Whenever the average ARP Availability from MSEE towards all peers is less than 100%.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**  
***The alert priority level is 2***  

2. BGP Availability  
Whenever the average BGP Availability from MSEE towards all peers is less than 100%.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**  
***The alert priority level is 2***  

3. Qos Drop Bits In Per Second  
Whenever the average Bits ingressing dropped for Azure expressroute circuits per second is greater than 1,000 bps.  
**This indicates potential issues with the data traffic to your Azure network through the express route.**  
***The alert priority level is 4***  

4. Qos Drop Bits Out Per Second  
Whenever the average Bits egressing dropped for Azure expressroute circuits per second is greater than 1,000 bps.  
**This indicates potential issues with the data traffic from your Azure network through the express route.**  
***The alert priority level is 4***  
