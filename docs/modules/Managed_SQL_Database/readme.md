# Deploy Azure SQL Database monitoring
This terraform script will deploy the following monitoring alerts for a SQL Database

1. Resource Health  
Resource Health status is no longer 'Available'

2. SQL Database Data Space Used Percent over 80%  
Whenever the maximum Data space used percent is greater than 80%

3. SQL Database Data Space Used Percent over 90%  
Whenever the maximum Data space used percent is greater than 90%

4. SQL Database Data Space Used Percent over 95%  
Whenever the maximum Data space used percent is greater than 95%

5. SQL Database CPU Percent high  
Whenever the average CPU percentage is greater than 90%

6. SQL Database CPU Percent critical  
Whenever the average CPU percentage is greater than 98%

7. SQL Database Workers Percent high  
Whenever the average Workers percentage is greater than 90%

8. SQL Database Workers Percent critical  
Whenever the average Workers percentage is greater than 90%

9. SQL Database Failed Connections  
Whenever the total Failed Connections : System Errors is greater than 1

10. SQL Database Deadlock    
Whenever the total Deadlocks is greater than 1