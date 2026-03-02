# Deploy Azure Load Balancers monitoring
## This terraform script will deploy the following monitoring alerts for Load Balancers

1. Allocated Snat Ports - Metric Alert  
Whenever the average total number of port allocated for SNAT is greater or less than dynamic criteria.  
**Azure does not provide a strict recommendation for SNAT port threshold because it depends on the specific network traffic patterns of your application. If your resource uses 40,000 SNAT ports out of the available 64,000 SNAT ports, you can set a warning alert when usage exceeds 80% of the SNAT ports (i.e., 51,200 ports).**
***The alert priority level is 2***  

2. Byte Count  
Total number of bytes passing through load balancer.  
**The threshold for ByteCount in a Metric Alert depends on the network traffic and data transfer patterns in your environment. ByteCount refers to the total number of bytes (data) transferred over the network, including both inbound and outbound traffic for a resource like a virtual machine, network interface, or application Assume a web server transfers an average of 500 MB (524,288,000 bytes) per minute. Exceeding the limit for 20%-30% should trigger alert.**  
***The alert priority level is 3***  

3. DipAvailability - Metric Alert 
Average Load Balancer health probe status per time duration  
**The DipAvailability metric in Azure typically refers to the availability of a Destination IP (Dip) in a Load Balancer or other networking-related resource. It helps monitor the health and reachability of a destination IP or service endpoint. 100% Availability is the ideal goal. Any dip below this should be investigated, especially in high-availability environments.**  
***The alert priority level is 3***  

4. Global Backend Availability - Metric Alert  
Global Backend Availability represents the percentage of time that the global backend services or instances (like virtual machines, app services, or APIs) are available and responding to requests.  
**In Azure typically monitors the availability of backend instances or services in a global context, such as in Traffic Manager or Application Gateway deployments with multiple backend pools across regions. This metric helps ensure that the backend servers or services in various geographic regions are available and responsive. 100% Availability is the ideal target.**  
***The alert priority level is 3***  

5. Packet Count - Metric Alert
Total number of packet passing through load balancer.  
**PacketCount refers to the total number of network packets (both inbound and outbound) handled by a resource (such as a virtual machine, network interface, or a web application). Normal Packet Count for VM is 50,000 packets per minute. Any spikes over 20%-30% should trigger alert.**  
***The alert priority level is 3***  

6. Snat Connection Count - Metric Alert  
Total number of new SNAT connections created within time period.  
**The SNAT Connection Count refers to the number of outbound connections being managed through SNAT. Azure provides a limited number of SNAT ports per VM or App Service, and when the limit is exceeded, further outbound connections can fail until old connections are closed or SNAT ports are freed up. App Services have specific SNAT port limits based on their plan. If the SNAT port limit is 128 for your plan, you can set a threshold at 90-100 connections.**  
***The alert priority level is 3***  

7. SYNCount - Metric Alert 
Number of syn packet which represent an attempt to establish tcp connection.  
**It's important to understand what the normal rate of SYN packets is in your environment. Some environments (like a high-traffic web server) may regularly see a high SYN count, while others (like an internal database) may expect very few. 5% more than the normal baseline traffic for your environment could be reasonable.**  
***The alert priority level is 3***  

8. Used SNAT Ports - Metric Alert  
Used SNAT Ports shows how many SNAT ports are in use out of the total available SNAT ports (64,000) for a given public IP address..  
**The UsedSNATPorts metric in Azure monitors the number of Source Network Address Translation (SNAT) ports currently in use by a given resource, such as a virtual machine or an app service making outbound connections.**  
***The alert priority level is 3***  

9. Vip Availability - Metric Alert  
In Azure typically measures the availability of the Virtual IP (VIP) of a load balancer, application gateway, or other public-facing service endpoints.  
**Critical Level: Trigger a critical alert when VipAvailability drops below 99% (indicating significant issues that may affect user experience).**  
***The alert priority level is 3***  
