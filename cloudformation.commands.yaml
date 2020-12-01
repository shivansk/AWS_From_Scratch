Cfn-linting: https://github.com/aws-cloudformation/cfn-python-lint
• cfn-lint template.yaml
• cfn-lint -t template.yaml

Multiple files can be linted by either specifying multiple specific files:
	• cfn-lint template1.yaml template2.yaml
	• cfn-lint -t template1.yaml template2.yaml
or by using wildcards (globbing):

Lint all yaml files in path:
	• cfn-lint path/*.yaml
  
Lint all yaml files in path and all subdirectories (recursive):
	• cfn-lint path/**/*.yaml


• Creating a stack

aws sts get-caller-identity
aws cloudformation validate-template --template-body file://template.yml
aws cloudformation create-stack --stack-name myteststack --template-body file://template.yml


• Describing and listing your stacks

aws cloudformation list-stacks
aws cloudformation describe-stacks
aws cloudformation delete-stack --stack-name myteststack1

• Viewing stack event history
aws cloudformation describe-stack-events --stack-name myteststack1
 
• Listing resources
aws cloudformation list-stack-resources --stack-name myteststack1

• Retrieving a template
aws cloudformation get-template --stack-name myteststack1

• Validating a template
aws cloudformation validate-template --template-url https://s3.amazonaws.com/cloudformation-templates-us-east-1/S3_Bucket.template
aws cloudformation validate-template --template-body file://03-01-cfn-ec2-instance-create.yml

• Uploading local artifacts to an S3 bucket
aws cloudformation package --template local-artifact-to-s3.yaml --s3-bucket mybucket --output yaml > local-artifact-to-s3.yaml

• Quickly deploying templates with transforms
aws cloudformation deploy --template 03-01-cfn-ec2-instance-create.yml  --stack-name myteststack1
aws cloudformation deploy --stack-name myteststack1 --template 03-01-cfn-ec2-instance-create.yml
aws cloudformation deploy --template /path_to_template/my-template.json --stack-name my-new-stack --parameter-overrides Key1=Value1 Key2=Value2

• Deleting a stack
aws cloudformation delete-stack --stack-name myteststack1

# Get AVZ
aws ec2 describe-availability-zones

# Play around with CloudFomration scripts on EC2 instances by using the below deploy command which creates a new changes set
aws cloudformation deploy --template 'file path to yaml you want to execute' --stack-name myteststack

# Get AVZ
aws ec2 describe-availability-zones
aws cloudformation deploy --template /Users/template.yml  myteststack7  --parameter-overrides MyRegionMap=ami-00a205cb8e06c3c4e  MyEnvironmentMap=t2.small
aws cloudformation deploy --template /Users/template.yml  myteststack8  --parameter-overrides ami-00a205cb8e06c3c4e
