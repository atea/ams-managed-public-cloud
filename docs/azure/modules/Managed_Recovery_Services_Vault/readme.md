# Deploy Azure Recovery Services Vault monitoring
## This terraform script will deploy the following monitoring alerts for a Recovery Services Vault

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**  
***The alert priority level is 2***  

2. Backup Health Events  
Whenever the count Backup Health Events is greater than 0  
**This indicates any issues or events affecting the health of backup processes, such as failures, warnings, or other relevant notifications.**  
***The alert priority Level is 2***  

3. Restore Health Events  
Whenever the count Restore Health Events is greater than 0  
**This indicates any issues or events affecting the health of restore processes, such as failures, warnings, or other relevant notifications.**  
***The alert priority Level is 3***  



