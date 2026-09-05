# Deploy Azure Virtual Network Gateways monitoring
## This terraform script will deploy the following monitoring alerts for Virtual Network Gateways

## VPN Gateway Alerts (deployed when gateway type is VPN)

1. Average Bandwidth  
Whenever the average Site-to-site bandwidth of a gateway in bytes per second is greater than 1,000,000,000 bps (1 Gbps).  
**This indicates potential higher data flow through the gateway than expected.**  
***The alert priority level is 5***  

2. Tunnel Average Bandwidth  
Whenever the average Tunnel Average Bandwidth is less than 1 bps.  
**This indicates that the VPN Gateway is potentially down, affecting all resources depending on this connection.**  
***The alert priority level is 2***  

3. Tunnel Egress Bytes  
Whenever the average Tunnel egress bytes is less than 1 byte.  
**This indicates that the VPN Gateway is potentially down, affecting all resources depending on this connection.**  
***The alert priority level is 2***  

4. Tunnel Egress Packet Drop Count  
Whenever the average Tunnel Egress Packet Drop Count is greater than 1,000.  
**This indicates if there are any disruptions in the flow of data through the VPN gateway, which may impact the availability of services dependent on the connection.**  
***The alert priority level is 5***  

5. Tunnel Egress Packet Drop TS Mismatch  
Whenever the average Tunnel Egress Packet Drop TS Mismatch is greater than 1,000.  
**This indicates if there are any disruptions in the flow of data through the VPN gateway, which may impact the availability of services dependent on the connection.**  
***The alert priority level is 5***  

6. Tunnel Ingress Bytes  
Whenever the average Tunnel Ingress bytes is less than 1 byte.  
**This indicates that the VPN Gateway is potentially down, affecting all resources depending on this connection.**  
***The alert priority level is 2***  

7. Tunnel Ingress Packet Drop Count  
Whenever the average Tunnel Ingress Packet Drop Count is greater than 1,000.  
**This indicates if there are any disruptions in the flow of data through the VPN gateway, which may impact the availability of services dependent on the connection.**  
***The alert priority level is 5***  

8. Tunnel Ingress Packet Drop TS Mismatch  
Whenever the average Tunnel Ingress Packet Drop TS Mismatch is greater than 1,000.  
**This indicates if there are any disruptions in the flow of data through the VPN gateway, which may impact the availability of services dependent on the connection.**  
***The alert priority level is 5***  

## ExpressRoute Gateway Alerts (deployed when gateway type is ExpressRoute)

9. Express Route Gateway Bits Per Second  
Whenever the average ExpressRoute Gateway Bits Per Second is less than 1 bps.  
**This indicates that the Expressroute Gateway is currently not available or functioning correctly.**  
***The alert priority level is 2***  

10. Express Route Gateway Cpu Utilization  
Whenever the average CPU Utilization of the ExpressRoute Gateway is greater than 80%.  
**This indicates that the Gateway is close to its maximum CPU capacity, exceeding this can lead to disruptions and traffic loss for resources depending on this connection.**  
***The alert priority level is 3*** 
