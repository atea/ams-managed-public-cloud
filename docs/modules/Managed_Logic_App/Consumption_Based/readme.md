# Deploy Azure Logic App monitoring
This terraform script will deploy the following monitoring alerts for a Logic App

1. Resource Health  
Resource Health status is no longer 'Available'

2. Logic Run Failure Percentage  
Triggered when the total Runs Failed is greater than 0

3. Run Latency Medium
Whenever the average Run Latency is greater or less than dynamic criteria

4. Run Latency High
Whenever the average Run Latency is greater or less than dynamic criteria



