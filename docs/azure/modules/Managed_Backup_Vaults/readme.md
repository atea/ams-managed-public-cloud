# Deploy Azure Backup Vaults
## This terraform script will deploy the following monitoring alerts for a Backup Vaults

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**    
***The alert priority level is 2*** 

2. Backup Health  
Whenever the count Backup Health Events is greater than 1.  
**The alert notifies you when there is at least one backup health issue, so you can quickly address potential problems with your backups.**  
***The alert priority Level is 2***  

3. Restore Health  
Triggered when the Whenever the count Restore Health Events is greater than 1.  
**The alert notifies you when there is at least one restore health issue, so you can quickly address potential problems with your restore processes.**  
***The alert priority Level is 2***  





