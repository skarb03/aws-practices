## 예제 실행(AWS에 stack 생성하기)

### ex03
```bash
$ aws cloudformation create-stack --stack-name myserver --template-body https://raw.githubusercontent.com/skarb03/aws-practices/main/02/ch04/04/ex03.json --parameters ParameterKey=KeyName,ParameterValue=mykey-s ParameterKey=VPC,ParameterValue=vpc-fc47d997 ParameterKey=InstanceType,ParameterValue=t2.micro

$ aws cloudformation describe-stacks --stack-name myserver --query Stacks[0].Outputs

$ aws cloudformation delete-stack --stack-name myserver

```