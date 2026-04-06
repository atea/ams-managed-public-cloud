# Deploy Azure Firewall monitoring
## This terraform script will deploy the following monitoring alerts for a Azure Firewall

1. Firewall Health  
Whenever the average Firewall Health is less than 100%.  
**Indicates the health of the firewall based on SNAT port availability. This measures the overall health and availability of the Azure Firewall, with deviations from expected values potentially indicating issues with the firewall's ability to process traffic.**  
***The alert priority level is 2***  

2. SNAT Port Utilization  
Whenever the average SNAT Port Utilization is greater than 80%.  
**This indicates that the Firewall has used up all its available ports for translating internal IP addresses to external ones, potentially causing issues with outgoing network connections.**  
***The alert priority level is 3***  

3. Throughput  
Whenever the average Throughput is greater than 10,000,000 bps (10 Mbps).  
**This indicates if there are any bottleneck in the flow of data through the Firewall, which may impact the availability of services behind it.**  
***The alert priority level is 4***  
