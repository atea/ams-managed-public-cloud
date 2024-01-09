# Deploy Azure SQL Elastic Pool monitoring
This terraform script will deploy the following monitoring alerts for a SQL Elastic Pool

1. Resource Health  
Resource Health status is no longer 'Available'

2. Data space used percent proactive  
Whenever the average Data space used percent is greater than 80%

3. Data space used percent high  
Whenever the average Data space used percent is greater than 90%

4. Data space used percent critical  
Whenever the average Data space used percent is greater than 95%

5. CPU percentage high  
Whenever the average CPU percentage is greater than 90%

6. CPU percentage critical  
Whenever the average CPU percentage is greater than 98%

7. Data space allocated percent proactive  
Whenever the maximum Data space allocated percent is greater than 80%

8. Data space allocated percent high  
Whenever the maximum Data space allocated percent is greater than 90%

9. Data space allocated percent critical  
Whenever the maximum Data space allocated percent is greater than 95%

10. Data IO percentage High  
Whenever the average Data IO percentage is greater than 90%

11. Data IO percentage Critical  
Whenever the average Data IO percentage is greater than 98%



