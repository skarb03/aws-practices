### ex05
```bash
$ aws cloudformation create-stack --stack-name myserver --template-body https://raw.githubusercontent.com/skarb03/aws-practices/main/02/ch05/03/ex05.json --parameters ParameterKey=KeyName,ParameterValue=mykey-s ParameterKey=VPC,ParameterValue=vpc-fc47d997 ParameterKey=InstanceType,ParameterValue=t2.micro --capabilities CAPABILITY_NAMED_IAM

$ aws cloudformation describe-stacks --stack-name myserver --query Stacks[0].Outputs

$ aws cloudformation delete-stack --stack-name myserver

```