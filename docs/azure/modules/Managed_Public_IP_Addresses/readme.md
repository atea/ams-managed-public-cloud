# Deploy Azure Public IP Addresses monitoring
## This terraform script will deploy the following monitoring alerts for Public IP Addresses

1. Bytes In DDoS  
Whenever the maximum Inbound bytes dropped DDoS is greater than 8,000,000 bytes.  
**This alert allows you to be notified if your public IP address is potentially affected by a continuous DDoS attack.**  
***The alert priority level is 5***  

2. If Under DDoS Attack  
Whenever the maximum value for Under DDoS attack or not is greater than 0.  
**This alert allows you to be notified if your public IP address is potentially affected by a DDoS attack.**  
***The alert priority level is 2***  

3. Packets In DDoS  
Whenever the total Inbound packets dropped DDoS is greater than or equal to 40,000 packets.  
**This alert allows you to be notified if your public IP address is potentially affected by a DDoS attack.**  
***The alert priority level is 4***  

4. TCP Bytes In DDoS  
Whenever the maximum Inbound TCP bytes DDoS is greater than 40,000 bytes.  
**This alert allows you to be notified if your public IP address is potentially affected by a DDoS attack.**  
***The alert priority level is 4***  

5. TCP Packets In DDoS  
Whenever the maximum Inbound TCP packets DDoS is greater than or equal to 40,000 packets.  
**This alert allows you to be notified if your public IP address is potentially affected by a DDoS attack.**  
***The alert priority level is 4***  

6. UDP Bytes In DDoS  
Whenever the maximum Inbound UDP bytes DDoS is greater than or equal to 40,000 bytes.  
**This alert allows you to be notified if your public IP address is potentially affected by a DDoS attack.**  
***The alert priority level is 4***  

7. UDP Packets In DDoS  
Whenever the maximum Inbound UDP packets DDoS is greater than or equal to 40,000 packets.  
**This alert allows you to be notified if your public IP address is potentially affected by a DDoS attack.**  
***The alert priority level is 4***  

8. Vip Availability  
Whenever the average IP Address availability per time duration is less than 90%.  
**This alert allows you to be notified if your public IP address availability is degraded.**  
***The alert priority level is 2***  
