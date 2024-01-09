# Deploy Azure Service Bus Namespace monitoring
This terraform script will deploy the following monitoring alerts for a Service Bus Namespace

1. Resource Health  
Resource Health status is no longer 'Available'

2. Dead-Lettered Messages  
Whenever the average count of dead-lettered messages in a Queue/Topic is greater than 2

3. Active Messages  
Whenever the average count of active messages in a Queue/Topic is greater than 2

4. Service Bus Messages  
Whenever the average count of messages in a Queue/Topic is greater than 2



