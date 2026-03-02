# Deploy Azure Traffic Manager Profiles monitoring
## This terraform script will deploy the following monitoring alerts for a Traffic Manager Profiles

1. Probe Agent Current Endpoint State By Profile Resource Id  
1 if an endpoint's probe status is "Enabled", 0 otherwise.  
**This indicates potential traffic manager endpoint is disabled, impacting operational efficiency and service availability.**  
***The alert priority level is 4***  

2. Qps By Endpoint  
Number of times a Traffic Manager endpoint was returned in the given time frame.  
**This indicates potential traffic manager endpoint is unavalible.**  
***The alert priority level is 4***  
