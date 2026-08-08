# Deploy Azure Traffic Manager Profiles monitoring
## This terraform script will deploy the following monitoring alerts for Traffic Manager Profiles

1. Probe Agent Current Endpoint State By Profile Resource Id  
Whenever the maximum endpoint probe status is less than 1 (1 if "Enabled", 0 if disabled).  
**This indicates potential traffic manager endpoint is disabled, impacting operational efficiency and service availability.**  
***The alert priority level is 4***  

2. Qps By Endpoint  
Whenever the total number of times a Traffic Manager endpoint was returned is less than or equal to 0.  
**This indicates potential traffic manager endpoint is unavailable.**  
***The alert priority level is 4***  
