# Deploy Container Instance monitoring
## This Terraform script will deploy the following monitoring alerts for Azure Container Instances (ACI)

1. Container CPU Usage

    Alerts when container CPU usage spikes high for 15 minutes.

    **This indicates high CPU usage that may impact the performance or availability of the container.**
    
    ***The alert priority level is 3*** 

2. Container Memory Usage

    Alerts when container memory usage spikes high for 15 minutes.

    **This alert identifies high memory utilization, which could result in performance degradation or out-of-memory errors.**

    ***The alert priority level is 3*** 

3. Container Network Input

    Alerts when network input utilization spikes high for 15 minutes.

    **This alert highlights significant incoming network traffic, which may indicate abnormal usage patterns or potential performance bottlenecks.**
    
    ***The alert priority level is 3***

4. Container Network Output

    Alerts when network output utilization spikes high for 15 minutes.

    **This alert highlights significant outgoing network traffic, which may indicate abnormal usage patterns or performance issues.**

    ***The alert priority level is 3***

