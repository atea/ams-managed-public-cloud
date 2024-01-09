# Deploy Azure Storage Account monitoring
This terraform script will deploy the following monitoring alerts for a Storage Account

1. Resource Health  
Resource Health status is no longer 'Available'

2. Availability  
The Storage Account is no longer available, please investigate

3. Egress  
Whenever the total Egress is greater or less than dynamic threshold

4. Ingress  
Whenever the total Ingress is greater or less than dynamic threshold

5. Blob Transactions  
The Storage Account Blob has deviations from the Normal level of Transactions

6. Success Server Latency  
The Storage Account Success Server Latency is more than 1000ms average over 5 minutes