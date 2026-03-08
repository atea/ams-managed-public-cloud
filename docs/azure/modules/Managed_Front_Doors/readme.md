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
