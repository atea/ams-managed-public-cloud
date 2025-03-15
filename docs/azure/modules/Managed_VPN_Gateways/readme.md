# Deploy Azure VPN Gateway monitoring
## This terraform script will deploy the following monitoring alerts for a VPN Gateway

1. Activity Log VPN Gateway Delete  
Activity Log, delete is succussed for VPN Gateway.  
**Alerts if the VPN Gateway is successfully deleted. Azure VPN Gateway is used for connections to sites and locations, if deleted impact’s function and security for multiple services in Azure.**  
***The alert priority level is 1***  

2. BGP Peer Status  
Whenever the average Health Probe Status is less than 100.  
**This tells us if the servers being used to handle incoming requests are working properly or not.**  
***The alert priority level is 3***  

3. Tunnel Average Bandwidth  
Metric Alert for VPN Gateway Bandwidth Utilization is less than 1.  
**This indicates that the VPN Gateway is potentially down, affecting all resources depending on this connection.**  
***The alert priority level is 1***  

4. Tunnel Egress Bytes  
Metric Alert for VPN Gateway tunnel egress bytes is less than 1.  
**This indicates that the VPN Gateway is potentially down, affecting all resources depending on this connection.**  
***The alert priority level is 1*** 

5. Tunnel Egress Packet Drop Count  
Metric Alert for VPN Gateway tunnel TunnelEgressPacketDropCount average greater than dynamic value.  
**This indicates if there are any disruptions in the flow of data through the VPN gateway, which may impact the availability of services dependent on the connection.**  
***The alert priority level is 4*** 

6. Tunnel Egress Packet Drop TS Mismatch  
Metric Alert for VPN Gateway tunnel TunnelEgressPacketDropTSMismatch average greater than dynamic value.  
**This indicates if there are any disruptions in the flow of data through the VPN gateway, which may impact the availability of services dependent on the connection.**  
***The alert priority level is 4*** 

7. Tunnel Ingress Bytes  
Metric Alert for VPN Gateway tunnel Ingress bytes is less than 1.  
**This indicates that the VPN Gateway is potentially down, affecting all resources depending on this connection.**  
***The alert priority level is 1*** 

8. Tunnel Ingress Packet Drop Count  
Metric Alert for VPN Gateway tunnel TunnelIngressPacketDropCount average greater than dynamic value.  
**This indicates if there are any disruptions in the flow of data through the VPN gateway, which may impact the availability of services dependent on the connection.**  
***The alert priority level is 4*** 

9. Tunnel Ingress Packet Drop TS Mismatch  
Metric Alert for VPN Gateway tunnel TunnelIngressPacketDropTSMismatch average greater than dynamic value.  
**This indicates if there are any disruptions in the flow of data through the VPN gateway, which may impact the availability of services dependent on the connection.**  
***The alert priority level is 4*** 
