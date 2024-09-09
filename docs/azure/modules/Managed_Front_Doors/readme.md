# Deploy Azure Front Door monitoring
## This terraform script will deploy the following monitoring alerts for a Front Door

1. Backend Health Percentage  
The percentage of successful health probes from the HTTP/S proxy to backends Less than 80%.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**  
***The alert priority level is 2***  

2. Backend Request Latency  
Whenever the average Total Latency is greater than 15000 milliseconds.  
**This measures the overall time delay experienced in a system, typically measured from the start of a process or action until its completion.**  
***The alert priority level is 4***  

3. Request Count  
Whenever the total Request Count is greater or less than dynamic criteria.  
**This refers to the total number of requests made to a specific service, endpoint, or resource within a defined period of time. This metric provides insight into the level of activity or demand placed on the service, helping to monitor and analyze its usage patterns, performance, and scalability.**  
***The alert priority level is 4***  

4. Total Latency  
Whenever the average Total Latency is greater than 25000 milliseconds.  
**This measures the overall time delay experienced in a system, typically measured from the start of a process or action until its completion.**  
***The alert priority level is 4***  

5. Origin Health Percentage  
Whenever the average Origin Health Percentage is less than 95%.  
**The percentage indicates the proportion of origin servers that are currently operational or healthy compared to the total number of origin servers configured in the system. Higher percentage is better.**  
***The alert priority level is 4***  

6. Percentage 5XX  
Whenever the average Percentage of 5XX is greater than 5%.  
**This metric represents the percentage of HTTP requests that resulted in server errors. This typically refers to a metric used to measure the frequency of server errors within a given system or service.**  
***The alert priority level is 4***  
