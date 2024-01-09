# Deploy Azure Key Vault monitoring
This terraform script will deploy the following monitoring alerts for a Key Vault

1. Resource Health  
Resource Health status is no longer 'Available'

2. Overall Vault Availability  
Triggered when the average availability of the Key Vault is less than 100%

3. Overall Vault Saturation high  
Triggered when the saturation (capacity) of the Key Vault is greater than 90%.

3. Overall Vault Saturation critical  
Triggered when the saturation (capacity) of the Key Vault is greater than 98%.

4. Total Service Api Hits  
Triggered based on dynamic criteria related to the total Service API hits for the Key Vault.

5. Overall Service Api Latency Medium  
 Triggered when the average Service API latency for the Key Vault is greater than dynamic criteria (Medium)

5. Overall Service Api Latency High  
 Triggered when the average Service API latency for the Key Vault is greater than dynamic criteria (High)

6. Total Service Api Results  
Triggered based on dynamic criteria related to the total results of the Service API for the Key Vault.




