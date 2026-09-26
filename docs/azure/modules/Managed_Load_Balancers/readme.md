# Deploy Azure Load Balancers monitoring
## This terraform script will deploy the following monitoring alerts for Load Balancers

1. Allocated Snat Ports - Metric Alert  
Whenever the average total number of ports allocated for SNAT is greater than 57,000 (Regional tier only).  
**Azure does not provide a strict recommendation for SNAT port threshold because it depends on the specific network traffic patterns of your application. If your resource uses 40,000 SNAT ports out of the available 64,000 SNAT ports, you can set a warning alert when usage exceeds 80% of the SNAT ports (i.e., 51,200 ports).**
***The alert priority level is 3***  

2. DipAvailability - Metric Alert  
Whenever the average Load Balancer health probe status is less than 90% (Regional tier only).  
**The DipAvailability metric in Azure typically refers to the availability of a Destination IP (Dip) in a Load Balancer or other networking-related resource. It helps monitor the health and reachability of a destination IP or service endpoint. 100% Availability is the ideal goal. Any dip below this should be investigated, especially in high-availability environments.**  
***The alert priority level is 2***  

3. Global Backend Availability - Metric Alert  
Whenever the average Global Backend Availability is less than 90% (Global tier only).  
**Global Backend Availability represents the percentage of time that the global backend services or instances (like virtual machines, app services, or APIs) are available and responding to requests. In Azure typically monitors the availability of backend instances or services in a global context, such as in Traffic Manager or Application Gateway deployments with multiple backend pools across regions. This metric helps ensure that the backend servers or services in various geographic regions are available and responsive. 100% Availability is the ideal target.**  
***The alert priority level is 2***  

4. Packet Count - Metric Alert  
Whenever the total Packet Count is greater than dynamic criteria (Low sensitivity, Regional tier only).  
**PacketCount refers to the total number of network packets (both inbound and outbound) handled by a resource (such as a virtual machine, network interface, or a web application). Normal Packet Count for VM is 50,000 packets per minute. Any spikes over 20%-30% should trigger alert.**  
***The alert priority level is 4***  

5. Snat Connection Count - Metric Alert  
Whenever the total number of new SNAT connections is greater than 10,000 (Regional tier only).  
**The SNAT Connection Count refers to the number of outbound connections being managed through SNAT. Azure provides a limited number of SNAT ports per VM or App Service, and when the limit is exceeded, further outbound connections can fail until old connections are closed or SNAT ports are freed up. App Services have specific SNAT port limits based on their plan. If the SNAT port limit is 128 for your plan, you can set a threshold at 90-100 connections.**  
***The alert priority level is 5***  

6. SYNCount - Metric Alert  
Whenever the total SYN packet count is greater than 10,000 (Regional tier only).  
**Number of syn packet which represent an attempt to establish tcp connection. It's important to understand what the normal rate of SYN packets is in your environment. Some environments (like a high-traffic web server) may regularly see a high SYN count, while others (like an internal database) may expect very few. 5% more than the normal baseline traffic for your environment could be reasonable.**  
***The alert priority level is 5***  

7. Used SNAT Ports - Metric Alert  
Whenever the average Used SNAT Ports is greater than 51,200 (Regional tier only).  
**Used SNAT Ports shows how many SNAT ports are in use out of the total available SNAT ports (64,000) for a given public IP address. The UsedSNATPorts metric in Azure monitors the number of Source Network Address Translation (SNAT) ports currently in use by a given resource, such as a virtual machine or an app service making outbound connections.**  
***The alert priority level is 2***  

8. Vip Availability - Metric Alert  
Whenever the average VIP Availability is less than 99%.  
**In Azure typically measures the availability of the Virtual IP (VIP) of a load balancer, application gateway, or other public-facing service endpoints. Critical Level: Trigger a critical alert when VipAvailability drops below 99% (indicating significant issues that may affect user experience).**  
***The alert priority level is 2***  
