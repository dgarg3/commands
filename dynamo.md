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
 ### aws dynamodb describe-backup --backup-arn **list your backup arn**
  ## describe dynamodb table 
 ### aws dynamodb describe-table --table-name **list your table name**
 ## scanning dynamodb table 
 ### aws dynamodb scan --table-name **list your table name**
 ## batch write dynamodb table
 ### aws dynamodb batch-write-item --request-items file://**list your filename**
 ## delete dynamodb table
 ### aws dynamodb delete-table --table-name **list your table name**
