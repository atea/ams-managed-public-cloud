# Deploy Azure Front Door monitoring
## This terraform script will deploy the following monitoring alerts for a Front Door

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**    
***The alert priority level is 2***  

2. Total Latency  
Whenever the average Total Latency is greater than 1000 milliseconds.  
**refers to the overall time delay experienced in a system, typically measured from the start of a process or action until its completion.**  
***The alert priority Level is 4***  

3. Origin Health Percentage  
Whenever the average Origin Health Percentage is less than 95%.  
**The percentage indicates the proportion of origin servers that are currently operational or healthy compared to the total number of origin servers configured in the system. Higher percentage is better**  
***The alert priority Level is 4***  

4. Percentage 5XX  
Whenever the average Percentage of 5XX is greater than 5%.  
**This metric represents the percentage of HTTP requests that resulted in server errors. This typically refers to a metric used to measure the frequency of server errors within a given system or service.**  
***The alert priority Level is 4***  

5. Request Count  
Whenever the total Request Count is greater or less than dynamic criteria.  
**This refers to the total number of requests made to a specific service, endpoint, or resource within a defined period of time. This metric provides insight into the level of activity or demand placed on the service, helping to monitor and analyze its usage patterns, performance, and scalability.**  
***The alert priority Level is 5***







