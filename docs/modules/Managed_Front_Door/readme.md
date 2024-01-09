# Deploy Azure Front Door monitoring
This terraform script will deploy the following monitoring alerts for a Front Door

1. Resource Health  
Resource Health status is no longer 'Available'

2. Total Latency   
Whenever the average Total Latency is greater than 1000 milliseconds

3. Origin Health Percentage  
Whenever the average Origin Health Percentage is less than 95%

4. Percentage 5XX  
Whenever the average Percentage of 5XX is greater than 5%

5. Request Count  
Whenever the total Request Count is greater or less than dynamic criteria







