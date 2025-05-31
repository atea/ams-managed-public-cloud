# Deploy Azure Public IP Adresses monitoring
## This terraform script will deploy the following monitoring alerts for a Public IP Adresses

1. Bytes In DDoS  
Metric Alert for Public IP Address Bytes IN DDOS Greater than 8000000.  
**This alert allows you to be notified if your public IP address is potentially affected by a continues DDoS attack.**  
***The alert priority level is 5***  

2. If Under DDoS Attack  
Metric Alert for Public IP Address Under Attack Greater than 0.  
**This alert allows you to be notified if your public IP address is potentially affected by a DDoS attack.**  
***The alert priority level is 2***  

3. Packets In DDoS  
Inbound packets DDoS Greater than 40000.  
**This alert allows you to be notified if your public IP address is potentially affected by a DDoS attack.**  
***The alert priority level is 5***  

4. TCP Bytes InDDoS  
Inbound TCP bytes DDoS Greater than 40000.  
**This alert allows you to be notified if your public IP address is potentially affected by a DDoS attack.**  
***The alert priority level is 4***  

5. TCP Packets In DDoS  
Inbound TCP packets DDoS Greater than 40000.  
**This alert allows you to be notified if your public IP address is potentially affected by a DDoS attack.**  
***The alert priority level is 4***  

6. UDP Bytes In DDoS  
Inbound UDP bytes DDoS Greater than 40000.  
**This alert allows you to be notified if your public IP address is potentially affected by a DDoS attack.**  
***The alert priority level is 4***  

7. UDP Packets In DDoS  
Inbound UDP packets DDoS Greater than 40000.  
**This alert allows you to be notified if your public IP address is potentially affected by a DDoS attack.**  
***The alert priority level is 3***  

8. Vip Availability  
Average IP Address availability per time duration less than 90%.  
**This alert allows you to be notified if your public IP address is potentially affected by a DDoS attack.**  
***The alert priority level is 3***  
