# Deploy Azure Application Gateway monitoring
This terraform script will deploy the following monitoring alerts for a Application Gateway

1. Resource Health  
Resource Health status is no longer 'Available'

2. Application Gateway Unhealthy Host Count  
Whenever the average Unhealthy Host Count is greater than 0

3. Application Gateway Failed requests  
Whenever the total Failed Requests is greater than 0

4. Application Gateway healthy host count  
Whenever the average Healthy Host Count is less than 1

5. Application Gateway Total time  
Whenever the average Application Gateway Total Time is greater or less than dynamic criteria




