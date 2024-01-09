# Deploy Azure Analysis Services monitoring
This terraform script will deploy the following monitoring alerts for a Analysis Services

1. Resource Health  
Resource Health status is no longer 'Available'

2. Memory Usage Medium  
Whenever the average memory_metric is greater than dynamic threshold (Medium)  

3. Memory Usage High  
Whenever the average memory_metric is greater than dynamic threshold (High)  

4. QPU Medium  
Whenever the average QPU is greater than dynamic threshold (Medium)

5. QPU High  
Whenever the average QPU is greater than dynamic threshold (High)





