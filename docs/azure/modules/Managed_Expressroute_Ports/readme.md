# Deploy Expressroute Ports monitoring
## This terraform script will deploy the following monitoring alerts for Expressroute Ports

1. Line Protocol 
Metric Alert for ER Direct Connection LineProtocol Less than 0.9.  
**This indicates that the ExpressRoute connection is potentially down and will affect connectivity for Expressroute connected networks.**  
***The alert priority level is 2***  

2. Port Bits In Per Second  
Metric Alert for ER Direct Connection PortBitsInPerSecond Less than 1.  
**This indicates that the ExpressRoute connection is potentially down and will affect connectivity for Expressroute connected networks.**  
***The alert priority level is 2***  

3. Port Bits Out Per Second  
Metric Alert for ER Direct Connection PortBitsOutPerSecond Less than 1.  
**This indicates that the ExpressRoute connection is potentially down and will affect connectivity for Expressroute connected networks.**  
***The alert priority level is 2***  

4. Rx Light Level  
Metric Alert for ER Direct Connection RxLightLevel Less than -10.  
**This indicates if there are any disruptions in the flow of data through the Expressroute, which may impact the availability of services hosted behind it.**  
***The alert priority level is 2***  

5. Tx Light Level  
Metric Alert for ER Direct Connection TxLightLevel Less than -10.  
**This indicates if there are any disruptions in the flow of data through the Expressroute, which may impact the availability of services hosted behind it.**  
***The alert priority level is 2***  
