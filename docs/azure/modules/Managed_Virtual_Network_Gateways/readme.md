# Deploy Azure Virtual Network Gateways monitoring
## This terraform script will deploy the following monitoring alerts for a Virtual Network Gateways

1. Average Bandwidth  
Site-to-site bandwidth of a gateway in bytes per second Greater than [X].  
**This indicates potential higher data flow through the gateway than expected.**  
***The alert priority level is 4***  

2. Express Route Gateway Bits Per Second  
Metric Alert for VNet Gateway Express Route Bits Per Second are less than 1.  
**This indicates that the Expressroute Gateway is currently not available or functioning correctly.**  
***The alert priority level is 1***
   
3. Express Route Gateway Cpu Utilization  
CPU Utilization of the ExpressRoute Gateway average is greater than 80%.  
**This indicates that the Gateway is close to its maximum CPU capacity, exceeding this can lead to disruptions and traffic loss for resources depending on this connection.**  
***The alert priority level is 2***

4. Tunnel Average Bandwidth  
Metric Alert for VPN Gateway Bandwidth Utilization is less than 1.  
**This indicates that the VPN Gateway is potentially down, affecting all resources depending on this connection.**  
***The alert priority level is 1***  

5. Tunnel Egress Bytes  
Metric Alert for VPN Gateway tunnel egress bytes is less than 1.  
**This indicates that the VPN Gateway is potentially down, affecting all resources depending on this connection.**  
***The alert priority level is 1*** 

6. Tunnel Egress Packet Drop Count  
Metric Alert for VPN Gateway tunnel TunnelEgressPacketDropCount average greater than dynamic value.  
**This indicates if there are any disruptions in the flow of data through the VPN gateway, which may impact the availability of services dependent on the connection.**  
***The alert priority level is 4*** 

7. Tunnel Egress Packet Drop TS Mismatch  
Metric Alert for VPN Gateway tunnel TunnelEgressPacketDropTSMismatch average greater than dynamic value.  
**This indicates if there are any disruptions in the flow of data through the VPN gateway, which may impact the availability of services dependent on the connection.**  
***The alert priority level is 4*** 

8. Tunnel Ingress Bytes  
Metric Alert for VPN Gateway tunnel Ingress bytes is less than 1.  
**This indicates that the VPN Gateway is potentially down, affecting all resources depending on this connection.**  
***The alert priority level is 1*** 

9. Tunnel Ingress Packet Drop Count  
Metric Alert for VPN Gateway tunnel TunnelIngressPacketDropCount average greater than dynamic value.  
**This indicates if there are any disruptions in the flow of data through the VPN gateway, which may impact the availability of services dependent on the connection.**  
***The alert priority level is 4*** 

9. Tunnel Ingress Packet Drop TS Mismatch  
Metric Alert for VPN Gateway tunnel TunnelIngressPacketDropTSMismatch average greater than dynamic value.  
**This indicates if there are any disruptions in the flow of data through the VPN gateway, which may impact the availability of services dependent on the connection.**  
***The alert priority level is 4*** 
