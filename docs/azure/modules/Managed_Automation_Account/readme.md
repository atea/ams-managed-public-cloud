# Deploy Azure Automation Account monitoring
## This terraform script will deploy the following monitoring alerts for a Automation Account

1. Resource Health  
Resource Health status is no longer 'Available'.  
**This indicates potential resource constraints impacting operational efficiency and service availability.**  
***The alert priority level is 2***  

2. Total Jobs Medium   
Whenever the total Total Jobs is greater or less than dynamic criteria (Medium).  
**This indicates instances where the number of jobs falls within a moderate range, potentially impacting workload management and operational efficiency.**  
***The alert priority level is 5***  

3. Total Jobs High  
Whenever the total Total Jobs is greater or less than dynamic criteria (Low).  
**This signals critical situations where the number of jobs exceeds or falls below the expected threshold, potentially affecting resource allocation and workflow execution.**  
***The alert priority level is 4***  

4. Account Total Update Deployment Runs Medium  
Whenever the total Total Update Deployment Runs is greater or less than dynamic criteria (Medium).  
**This indicates instances where the number of update deployment runs for the account falls within a moderate range, potentially impacting deployment efficiency and system maintenance.**  
***The alert priority level is 5***  

5. Account Total Update Deployment Runs High  
Whenever the total Total Update Deployment Runs is greater or less than dynamic criteria (Low).  
**This signals critical situations where the number of update deployment runs for the account exceeds or falls below the expected threshold, potentially indicating deployment issues or operational challenges.**  
***The alert priority level is 4***  

6. Total Update Deployment Machine Runs Medium  
Whenever the total Total Update Deployment Machine Runs is greater or less than dynamic criteria (Medium).  
**This indicates instances where the number of update deployment machine runs falls within a moderate range, potentially impacting deployment performance and system reliability.**  
***The alert priority level is 5***  

7. Total Update Deployment Machine Runs High  
Whenever the total Total Update Deployment Machine Runs is greater or less than dynamic criteria (Low).  
**This signals critical situations where the number of update deployment machine runs exceeds or falls below the expected threshold, potentially indicating deployment failures or infrastructure issues.**  
***The alert priority level is 4***  





