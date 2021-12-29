# **commands**
## how to scan the table
### aws dynamodb scan --table-name **list your table name**
## Delete Items from the table by inputting json file with partition and sort key
### aws dynamodb delete-item --table-name <table name> --key file://**enter your filename**
## query Items from the table by inputting json file with partition and field which is not sort key  
### aws dynamodb query --table-name **list your table name** --key-condition-expression "**list your primary key name** = :v1" --filter-expression "**list your field  name** <= :v2" --expression-attribute-values file://**enter your file name**
## backup dynamodb table 
### aws dynamodb create-backup --table-name **list your table name** --backup-name **list your backup name**
 ## describe dynamodb table backup 
 aws dynamodb describe-backup --backup-arn **list your backup arn**
