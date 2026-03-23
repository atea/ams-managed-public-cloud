# Deploy Azure Private DNS zone monitoring
## This terraform script will deploy the following monitoring alerts for a Private DNS zone

1. Record Set Capacity Utilization  
Whenever the maximum Record Set Capacity Utilization is greater than or equal to 60%.  
**This alert is to prevent reaching the record set limit for DNS zones.**  
***The alert priority level is 3***  

2. Record Set Count  
Whenever the maximum Number of Record Sets in a Private DNS zone is greater than 18,750.  
**This alert is to prevent reaching the record set limit for DNS zones.**  
***The alert priority level is 3***  

3. Virtual Network Link Capacity Utilization  
Whenever the maximum Virtual Network Link Capacity Utilization is greater than or equal to 80%.  
**This alert is to prevent reaching the network link limit for DNS zones.**  
***The alert priority level is 3***  

4. Virtual Network With Registration Capacity Utilization  
Whenever the maximum Virtual Network With Registration Capacity Utilization is greater than or equal to 80%.  
**This alert is to prevent reaching the network link limit with auto registration enabled for DNS zones.**  
***The alert priority level is 3***  
