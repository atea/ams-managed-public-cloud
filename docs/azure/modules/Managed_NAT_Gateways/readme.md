# Deploy Azure NAT Gateway monitoring
## This terraform script will deploy the following monitoring alerts for a NAT Gateway

1. Byte Count  
Total number of Bytes transmitted within time period Greater than [X].  
**This indicates that expected traffic through the NAT gateway is greater than expected.**  
***The alert priority level is 5***  

2. Data path Availability  
NAT Gateway Datapath Availability Less than 90%.  
**This tells us if there is a shortage off available outbound/inbound endpoints for traffic flow through the NAT gateway.**  
***The alert priority level is 4***  

3. Packet Drop Count  
Count of dropped packets Greater than 5.  
**This indicates increase in packet loss through the data gateway and might affect services behind it.**  
***The alert priority level is 2***  

4. Total Connection Count  
Total number of active SNAT connections Greater than 50000.  
**This shortage of availability on SNAT ports on NAT gateway.**  
***The alert priority level is 3***  
