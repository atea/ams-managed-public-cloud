# Deploy Azure DNS zone monitoring
## This terraform script will deploy the following monitoring alerts for a DNS zone

1. Query Volume  
Whenever the total number of queries served for a DNS zone is greater or less than dynamic criteria (Low sensitivity).  
**Monitors the query volume to detect abnormal spikes or drops in DNS traffic that may indicate issues or attacks.**  
***The alert priority level is 3***  

2. Record Set Capacity Utilization (Priority 3)  
Whenever the maximum Record Set Capacity Utilization is greater than or equal to 90%.  
**This alert provides an early warning to prevent reaching the record set limit for DNS zones.**  
***The alert priority level is 3***  

3. Record Set Capacity Utilization (Priority 4)  
Whenever the maximum Record Set Capacity Utilization is greater than 80%.  
**This alert is a secondary notification tier to prevent reaching the record set limit for DNS zones.**  
***The alert priority level is 4***  
