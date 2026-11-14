# Deploy Azure Virtual Machine monitoring  
## This terraform script will deploy the following monitoring alerts for Azure Virtual Machines  

1. VM Availability  
Measure of Availability of Virtual machines over time.  
**The deployed alert monitors the availability of virtual machines in Azure. It triggers when the average availability metric (VmAvailabilityMetric) drops below 1 over a 5-minute window, indicating potential downtime.**  
***The alert priority Level is 3***  

2. CPU over 98%  
Triggers when VM CPU usage exceeds 98% for 15 minutes.  
**The deployed alert monitors CPU usage on virtual machines and triggers a Priority 2 (P2) alert if the average CPU usage exceeds 98% over a 15-minute window. This helps identify performance bottlenecks or overloaded VMs, prompting immediate action.**  
***The alert priority Level is 2***  

3. CPU over 90%  
Triggers when VM CPU usage exceeds 90% for 15 minutes.  
**The deployed alert monitors CPU usage on virtual machines and triggers a Priority 4 (P4) alert if the average CPU usage exceeds 90% over a 15-minute window. This helps identify performance bottlenecks or overloaded VMs.**  
***The alert priority Level is 4***  

4. OS Disk IOPS over 90%  
Triggers when OS Disk IOPS usage exceeds 90% for 15 minutes.  
**The deployed alert monitors the OS disk IOPS consumption on virtual machines. It triggers when the average percentage of IOPS consumed exceeds 90% over a 15-minute window, indicating potential disk performance saturation. When this threshold is breached, an alert is raised**
***The alert priority Level is 4***

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
**The deployed alert monitors the Data disk IOPS consumption on virtual machines. It triggers when the average percentage of IOPS consumed exceeds 90% over a 15-minute window, indicating potential disk performance saturation. When this threshold is breached, an alert is raised**  
***The alert priority Level is 4***

8. Data Disk IOPS over 98%  
Triggers when Data Disk IOPS usage exceeds 98% for 15 minutes.  
**The deployed alert monitors the Data disk IOPS consumption on virtual machines. It triggers when the average percentage of IOPS consumed exceeds 98% over a 15-minute window, indicating potential disk performance saturation. When this threshold is breached, an alert is raised**  
***The alert priority Level is 2***  

9. Syslog Critical event (Linux)  
Triggers when there's a critical or higher level event in Syslog
**The deployed alert monitors critical Syslog events on virtual machines. It triggers a severity 2 alert if any log entry with a severity level of emergency, alert, or critical is detected within the last 5 minutes. When such an event occurs, the alert sends a notification to the configured action group for immediate attention.**  
***The alert priority Level is 2***  

9. Event log Critical event (Windows)  
Triggers when there's a critical or higher level event in Syslog  
**The deployed alert monitors critical Syslog events on virtual machines. It triggers a severity 2 alert if any log entry with a severity level of emergency, alert, or critical is detected within the last 5 minutes. When such an event occurs, the alert sends a notification to the configured action group for immediate attention.**  
***The alert priority Level is 2***  