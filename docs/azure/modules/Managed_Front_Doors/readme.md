# Deploy Azure CDN Profile monitoring
## This terraform script will deploy the following monitoring alerts for CDN Profiles (Front Door)

1. Request Count  
Whenever the total Request Count is greater than 10.  
**This refers to the total number of requests made to a specific service, endpoint, or resource within a defined period of time. This metric provides insight into the level of activity or demand placed on the service, helping to monitor and analyze its usage patterns, performance, and scalability.**  
***The alert priority level is 4***  

2. Total Latency  
Whenever the average Total Latency is greater than 25,000 milliseconds (25 seconds).  
**This measures the overall time delay experienced in a system, typically measured from the start of a process or action until its completion.**  
***The alert priority level is 4***   
