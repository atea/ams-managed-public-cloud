# Deploy Azure Event Hub monitoring  
## This terraform script will deploy the following monitoring alerts for a Analysis Services  

1. Cpu percentage  
Whenever the average Cpu percentage is greater than 95%  
**This indicates high CPU used to monitor the CPU usage of cluster resources and trigger notifications or actions when the usage exceeds a predefined threshold.**  
***The alert priority Level is 3***  

2. Memory Working Set Percentage  
Whenever the average Memory Working Set Percentage is greater than 80%  
**This indicates the percentage of memory actively being used by workloads, helping identify potential memory pressure in the cluster.**  
***The alert priority level is 3***  

3. AKS - Disk Usage Percentage  
Whenever the average Disk Used Percentage is greater than 80%  
**This monitors the percentage of disk space used by resources within the cluster, ensuring storage availability and performance..**  
***The alert priority level is 3***  

4. AKS - Number of pods by phase  
Whenever the average Number of pods by phase is greater than 0.  
**This monitors the count of pods in specific phases (e.g., Running, Pending, Failed) to track the state of workloads in the cluster**  
***The alert priority Level is 3***  

5. AKS - Statuses for various node conditions 
Whenever the total Statuses for various node conditions is greater than 0.  
**Monitors the health and status of nodes in the cluster to ensure the underlying infrastructure is functioning properly.**  
***The alert priority Level is 3*** 
