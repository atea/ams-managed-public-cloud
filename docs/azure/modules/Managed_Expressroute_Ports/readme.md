# Deploy Expressroute Ports monitoring
## This terraform script will deploy the following monitoring alerts for Expressroute Ports

1. Line Protocol 
Metric Alert for ER Direct Connection LineProtocol Less than 0,9.  
**This indicates that the ExpressRoute connection is potentially down and will affect connectivity for Expressroute connected networks.**  
***The alert priority level is 1***  

2. Port Bits In Per Second  
Metric Alert for ER Direct Connection BitsInPerSecond Less than 1.  
**This indicates that the ExpressRoute connection is potentially down and will affect connectivity for Expressroute connected networks.**  
***The alert priority level is 1***  

3. Port Bits Out Per Second  
Metric Alert for ER Direct Connection BitsOutPerSecond Less than 1.  
**This indicates that the ExpressRoute connection is potentially down and will affect connectivity for Expressroute connected networks.**  
***The alert priority level is 1***  

4. Rx Light Level - High  
Metric Alert for ER Direct Connection RxLightLevel High Greater than 0.  
**This indicates if there are any disruptions in the flow of data through the Expressroute, which may impact the availability of services hosted behind it.**  
***The alert priority level is 2***  

5. Rx Light Level - Low  
Metric Alert for ER Direct Connection RxLightLevel Low Less than -10.  
**This indicates if there are any disruptions in the flow of data through the Expressroute, which may impact the availability of services hosted behind it.**  
***The alert priority level is 2***  

6. Tx Light Level - High  
Metric Alert for ER Direct Connection TxLightLevel High Greater than 0.  
**This indicates if there are any disruptions in the flow of data through the Expressroute, which may impact the availability of services hosted behind it.**  
***The alert priority level is 2***  

7. Tx Light Level - Low  
Metric Alert for ER Direct Connection TxLightLevel Low 0.  
**This indicates if there are any disruptions in the flow of data through the Expressroute, which may impact the availability of services hosted behind it.**  
***The alert priority level is 2***  
