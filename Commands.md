---
Terrraform Commands
---
$ terraform init
$ terraform plan
$ terraform apply
$ terraform destroy

// Configure multiple AWS account
$ aws configure --profile account1
$ aws configure --profile account2
// example
aws configure --profile AWSAcc
AWS Access Key ID [None]: ********
AWS Secret Access Key [None]: *********
Default region name [None]: eu-west-1
Default output format [None]: json

$ aws configure list
      Name                    Value             Type    Location
      ----                    -----             ----    --------
   profile                <not set>             None    None
access_key     ****************NVLS shared-credentials-file    
secret_key     ****************R/OD shared-credentials-file    
    region                eu-west-1      config-file    ~/.aws/config
    
$ aws configure list
$ export AWS_DEFAULT_PROFILE=AWSAcc
$ aws configure list
