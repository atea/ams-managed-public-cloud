# Deploy Azure Application Gateway monitoring
## This terraform script will deploy the following monitoring alerts for an Application Gateway

1. Application Gateway Total time  
Whenever the average Application Gateway Total Time is greater or less than dynamic criteria.  
**This measures the overall performance of the application gateway in processing requests, with deviations from expected values potentially indicating issues with latency or processing efficiency.**  
***The alert priority level is 3***  

2. Backend Last Byte Response Time  
Whenever the average Application Gateway Total Time is greater or less than dynamic criteria.  
**This measures the overall performance of the application gateway in processing requests, with deviations from expected values potentially indicating issues with latency or processing efficiency.**  
***The alert priority level is 3***  

3. Backend Connect Time  
Whenever the average Application Gateway Total Time is greater or less than dynamic criteria.  
**This measures the overall performance of the application gateway in processing requests, with deviations from expected values potentially indicating issues with latency or processing efficiency.**  
***The alert priority level is 3***  

4. Backend First Byte Response Time  
Whenever the average Application Gateway Total Time is greater or less than dynamic criteria.  
**This measures the overall performance of the application gateway in processing requests, with deviations from expected values potentially indicating issues with latency or processing efficiency.**  
***The alert priority level is 4***  

5. Backend Response Status  
Whenever the total Failed Requests is greater than 10.  
**This alert to instances where requests to the application gateway have failed, potentially indicating issues with connectivity, configuration, or backend services.**  
***The alert priority level is 3***  

6. Capacity Units  
Capacity Unit utilization crosses 75% of peak usage.  
**Capacity units represent overall gateway utilization in terms of throughput, compute, and connection count. Check your maximum capacity unit usage in the last one month and set alert if it crosses 75% of it.**  
***The alert priority level is 3***  

7. Compute Units  
Compute Unit utilization crosses 75% of average usage.  
**Compute unit is the measure of compute utilization of your Application Gateway. Check your average compute unit usage in the last one month and set alert if it crosses 75% of it.**  
***The alert priority level is 3***  

8. Cpu Utilization  
CPU utilization average is higher than 80% utalization.  
**This alert is to prevent CPU throttle and proactive response to increase capacity.**  
***The alert priority level is 4***  

9. Current Connections  
Whenever the threshold of [X] is exceeded in number of current connections.  
**This alert whenever the threshold of X is exceeded in number of current connections, where X is configured depending on environment.**  
***The alert priority level is 4***  

10. Failed requests  
Whenever the total Failed Requests is greater than 10.  
**This alert to instances where requests to the application gateway have failed, potentially indicating issues with connectivity, configuration, or backend services.**  
***The alert priority level is 4***  

11. Healthy host count  
Whenever the average Healthy Host Count is less than 1.  
**This indicates situations where all backend hosts are deemed unhealthy, potentially causing service disruptions and requiring immediate attention.**  
***The alert priority level is 2***  

12. Response Status  
Whenever the total Failed Requests is greater than 10.  
**This alert to instances where requests to the application gateway have failed, potentially indicating issues with connectivity, configuration, or backend services.**  
***The alert priority level is 2***  

13. Throughput  
Whenever the Number of bytes per second the Application Gateway is greater than [X].  
**Alerts when the dataflow of through the gateway is higher than the threshold of [X].**  
***The alert priority level is 4***  

14. Total Requests  
Whenever the total Count of successful requests that Application Gateway has served is greater than [X].  
**Alerts Whenever the total Count of successful requests that Application Gateway has served is greater than [X].**  
***The alert priority level is 4***  

15. Unhealthy Host Count  
Whenever the average Unhealthy Host Count is greater than 0.  
**This indicates potential issues with the health or availability of backend hosts, which may impact the overall performance and reliability of the application.**  
***The alert priority level is 3***  

16. AzwafSecRule  
Matched Managed Rules greater than 75.  
**Trend for.**  
***The alert priority level is 4***  
AzwafSecRule
