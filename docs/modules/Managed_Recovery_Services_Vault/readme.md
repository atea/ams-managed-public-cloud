# Deploy Azure Recovery Services Vault monitoring
This terraform script will deploy the following monitoring alerts for a Recovery Services Vault

1. Resource Health  
Resource Health status is no longer 'Available'

2. Backup Health Events  
Whenever the count Backup Health Events is greater than 0

3. Restore Health Events  
Whenever the count Restore Health Events is greater than 0



