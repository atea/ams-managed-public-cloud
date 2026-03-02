# Deploy Event Grid monitoring
## This terraform script will deploy the following monitoring alerts for an Event Grid Topics

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**  
***The alert priority level is 2***  

2. Dead Lettered Events  
Whenever the total Dead Lettered Events is greater than dynamic criteria.  
**This alert indicates instances where messages have failed to be processed and have been moved to a dead-letter queue. Addressing these events promptly ensures the smooth flow of message processing and maintains system reliability.**  
***The alert priority level is 5***  

3. Delivery Failed Events  
Whenever the total Delivery Failed Events is greater than dynamic criteria.  
**This alert highlights instances where message delivery has failed, potentially impacting critical business processes.**  
***The alert priority level is 4***  

4. Publish Failed Events  
Whenever the total Publish Failed Events is greater than dynamic criteria.  
**This alert signifies instances where message publishing has encountered failures, potentially affecting the dissemination of important information.**  
***The alert priority level is 4***  

5. Topics Dropped Events  
Whenever the total Dropped Events is greater than dynamic criteria.  
**This alert indicates instances where messages have been dropped due to system limitations or errors, potentially resulting in data loss or incomplete processing. Addressing these events promptly helps maintain data integrity and system reliability.**  
***The alert priority level is 3***  