# Deploy Azure Expressroute Gateway monitoring
## This terraform script will deploy the following monitoring alerts for an Expressroute Gateway

1. ER Gateway Connection Bits In Per Second  
ER Gateway Connection Bits In Per Second average is less than 1.  
**This indicates that the ExpressRoute Gateway connection is potentially down and will affect connectivity for Expressroute connected networks.**  
***The alert priority level is 1***  

2. ER Gateway Connection Bits Out Per Second  
ER Gateway Connection Bits Out Per Second average is less than 1.  
**This indicates that the ExpressRoute Gateway connection is potentially down and will affect connectivity for Expressroute connected networks.**  
***The alert priority level is 1***  

3. CPU Usage  
CPU utilization average is higher than 80% utilization.  
**This alert is to prevent CPU throttle and proactive response to increase capacity if needed.**  
***The alert priority level is 2***  
