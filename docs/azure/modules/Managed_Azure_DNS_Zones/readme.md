# Deploy Azure DNS zone monitoring
## This terraform script will deploy the following monitoring alerts for a DNS zone

1. Query Volume  
Number of queries served for a DNS zone.  
**This Number of queries served for a DNS zone.**  
***The alert priority level is 3***  

2. Record Set Capacity Utilization  
Record Set Capacity Utilization average is higher than 60% utilization.  
**This alert is to prevent reaching the record set limit for DNS zones.**  
***The alert priority level is 4***  
