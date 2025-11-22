# Deploy Azure Private DNS zone monitoring
## This terraform script will deploy the following monitoring alerts for a Private DNS zone

1. Record Set Capacity Utilization  
Record Set Capacity Utilization average is higher than 60% utilization.  
**This alert is to prevent reaching the record set limit for DNS zones.**  
***The alert priority level is 3***  

2. Record Set Count  
Number of Record Sets in a Private DNS zone greater than 18750.  
**This alert is to prevent reaching the record set limit for DNS zones.**  
***The alert priority level is 3***  

3. Virtual Network Link Capacity Utilization  
Record Set Capacity Utilization average is higher than 80% utilization.  
**This alert is to prevent reaching the network link limit for DNS zones.**  
***The alert priority level is 3***  

4. Virtual Network With Registration Capacity Utilization  
Record Set Capacity Utilization average is higher than 80% utilization.  
**This alert is to prevent reaching the network link limit with auto registration enabled for DNS zones.**  
***The alert priority level is 3***  
