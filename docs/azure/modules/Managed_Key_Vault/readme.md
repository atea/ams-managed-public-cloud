# Deploy Azure Key Vault monitoring
## This terraform script will deploy the following monitoring alerts for a Key Vault

1. Overall Vault Availability  
Triggered when the average availability of the Key Vault is less than 100%.  
**This indicates the percentage of time the Azure Key Vault service is available for use.**  
***The alert priority Level is 2***  

2. Overall Vault Saturation high  
Triggered when the saturation (capacity) of the Key Vault is greater than 90%.  
**This indicates a high level of resource utilization within the Azure Key Vault service, potentially impacting its performance and responsiveness.**  
***The alert priority Level is 3***  

3. Overall Vault Saturation critical  
Triggered when the saturation (capacity) of the Key Vault is greater than 98%.  
**This indicates a critical level of resource utilization within the Azure Key Vault service, significantly impacting its performance and potentially causing service disruptions.**  
***The alert priority Level is 2***  

4. Total Service Api Hits  
Triggered based on dynamic criteria related to the total Service API hits for the Key Vault.  
**This represents the cumulative count of requests made to the service's API endpoints within a specified time frame.**  
***The alert priority Level is 5***  

5. Overall Service Api Latency Medium  
 Triggered when the average Service API latency for the Key Vault is greater than dynamic criteria (Medium)  
 **This indicates a moderate level of latency experienced when accessing the service's API endpoints, potentially impacting user experience or system responsiveness.**  
 ***The alert priority Level is 3***  

5. Overall Service Api Latency High  
 Triggered when the average Service API latency for the Key Vault is greater than dynamic criteria (Low)  
 **This indicates a high level of latency experienced when accessing the service's API endpoints, significantly impacting user experience or system responsiveness.**  
 ***The alert priority Level is 2***  

6. Total Service Api Results  
Triggered at 20000 total results over 1 minutes of the Service API for the Key Vault.  
**This represents the cumulative count of results returned by the service's API endpoints within a specified time frame.**  
***The alert priority Level is 5***




