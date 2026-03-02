# Deploy Azure Firewall monitoring
## This terraform script will deploy the following monitoring alerts for a Azure Firewall

1. Activity Log Azure Firewall Delete  
Activity Log, delete is succussed for Azure firewall.  
**Alerts if the firewall is deleted successfully deleted. Azure firewall is a central security feature that if deleted impact’s function and security for multiple services in Azure.**  
***The alert priority level is 1***  

2. Firewall Health  
Indicates the health of the firewall based on SNAT port availability, Possible values are Healthy, Degraded, Unhealthy.  
**This measures the overall performance of the application gateway in processing requests, with deviations from expected values potentially indicating issues with latency or processing efficiency.**  
***The alert priority level is 1***  

3. SNAT Port Utilization  
Whenever the Used SNAT Ports is greater than 80%.  
**This indicates that the Firewall has used up all its available ports for translating internal IP addresses to external ones, potentially causing issues with outgoing network connections.**  
***The alert priority level is 2***  

4. Throughput  
Rate of data traversing the firewall per second, threshold set in bits per second depending on Firewall.  
**This indicates if there are any bottleneck in the flow of data through the Firewall, which may impact the availability of services behind it.**  
***The alert priority level is 3***  
