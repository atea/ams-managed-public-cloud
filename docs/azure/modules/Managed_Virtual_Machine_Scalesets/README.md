# Deploy Azure Virtual Machine Scaleset monitoring  
## This terraform script will deploy the following monitoring alerts for Azure Virtual Machine Scalesets  

1. CPU over 98%  
Triggers when VM CPU usage exceeds 98% for 15 minutes.  
**The deployed alert monitors CPU usage on VMSS and triggers a Priority 2 (P2) alert if the average CPU usage exceeds 98% over a 15-minute window. This helps identify performance bottlenecks or overloaded VMs, prompting immediate action.**  
***The alert priority Level is 2***  

2. CPU over 90%  
Triggers when VM CPU usage exceeds 90% for 15 minutes.  
**The deployed alert monitors CPU usage on VMSS and triggers a Priority 4 (P4) alert if the average CPU usage exceeds 90% over a 15-minute window. This helps identify performance bottlenecks or overloaded VMs.**  
***The alert priority Level is 4***  

3. OS Disk IOPS over 90%  
Triggers when OS Disk IOPS usage exceeds 90% for 15 minutes.  
**The deployed alert monitors the OS disk IOPS consumption on VMSS. It triggers when the average percentage of IOPS consumed exceeds 90% over a 15-minute window, indicating potential disk performance saturation. When this threshold is breached, an alert is raised**  
***The alert priority Level is 4***  

4. OS Disk IOPS over 98%  
Triggers when OS Disk IOPS usage exceeds 90% for 15 minutes.  
**The deployed alert monitors the OS disk IOPS consumption on VMSS. It triggers when the average percentage of IOPS consumed exceeds 98% over a 15-minute window, indicating potential disk performance saturation. When this threshold is breached, an alert is raised**
***The alert priority Level is 2***

5. Data Disk Bandwidth over 90%  
Data Disk Bandwidth Consumed Percentage exceeds 90% for 15 minutes.  
**The deployed alert monitors the data disk bandwidth consumption on virtual machines. It raises an alert if the average bandwidth consumed exceeds 90% over a 15-minute window, helping to detect potential disk throughput bottlenecks.**  
***The alert priority Level is 4***

6. Data Disk Bandwidth over 98%  
Data Disk Bandwidth Consumed Percentage exceeds 98% for 15 minutes.  
**The deployed alert monitors the data disk bandwidth consumption on virtual machines. It raises an alert if the average bandwidth consumed exceeds 90% over a 15-minute window, helping to detect potential disk throughput bottlenecks, prompting immediate action.**  
***The alert priority Level is 2***

7. Data Disk IOPS over 90%  
Triggers when Data Disk IOPS usage exceeds 90% for 15 minutes.  
**The deployed alert monitors the Data disk IOPS consumption on VMSS. It triggers when the average percentage of IOPS consumed exceeds 90% over a 15-minute window, indicating potential disk performance saturation. When this threshold is breached, an alert is raised**  
***The alert priority Level is 4***

8. Data Disk IOPS over 98%  
Triggers when Data Disk IOPS usage exceeds 98% for 15 minutes.  
**The deployed alert monitors the Data disk IOPS consumption on VMSS. It triggers when the average percentage of IOPS consumed exceeds 98% over a 15-minute window, indicating potential disk performance saturation. When this threshold is breached, an alert is raised**  
***The alert priority Level is 2***  

9. Available memory under 2%  
Triggers when the VMSS has less than 2% memory left (98% memory utilization)  
**The deployed alert monitors the memory usage of the VMSS. It triggers when the average memory percentage left is under 2% over a 5-minute window. This helps identify performance bottlenecks or overloaded VMSS, prompting immediate action.**  
***The alert priority Level is 2***

9. Available memory under 10%  
Triggers when the VMSS has less than 10% memory left (90% memory utilization)  
**The deployed alert monitors the memory usage of the VMSS. It triggers when the average memory percentage left is under 10% over a 15-minute window. This helps identify performance bottlenecks or overloaded VMSS, prompting immediate action.**  
***The alert priority Level is 4***