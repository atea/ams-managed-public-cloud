# Deploy Azure Load Balancer monitoring
## This terraform script will deploy the following monitoring alerts for a Load Balancer

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**    
***The alert priority level is 2***  

2. Load Balancer Health Probe Status  
Whenever the average Health Probe Status is less than 100.  
**This tells us if the servers being used to handle incoming requests are working properly or not.**  
***The alert priority Level is 3***  

3. Load Balancer Used SNAT Ports  
Whenever the average Used SNAT Ports is greater than 900.  
**This indicates that the load balancer has used up all its available ports for translating internal IP addresses to external ones, potentially causing issues with outgoing network connections.**  
***The alert priority Level is 5***  

4. Load Balancer Data Path Availability  
Whenever the average Data Path Availability is less than 100.  
**This indicates if there are any disruptions in the flow of data through the load balancer, which may impact the availability of services hosted behind it.**  
***The alert priority Level is 3***  

  > *Source Network Address Translation (SNAT) is a way for a device, like a router or firewall, to change the sender's address in a message as it travels across a network. It's often used when multiple devices in a private network share one public internet address. SNAT swaps the private addresses of these devices with a single public address, making it look like all the requests are coming from one place. This helps manage internet traffic efficiently.