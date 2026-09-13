# Deploy Azure Route Tables monitoring
## This terraform script will deploy the following monitoring alerts for Route Tables

1. Activity Log Route Table Update  
Activity Log alert when route table route write succeeds (operation: Microsoft.Network/routeTables/routes/write).  
**This tracks and verifies route changes.**  
***The alert priority level is 2***  
