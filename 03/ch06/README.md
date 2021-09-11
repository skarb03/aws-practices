

## ex02 

#aws cloudformation create-stack --stack-name myapp --template-body https://raw.githubusercontent.com/skarb03/aws-practices/main/03/ch06/ex02.json --parameters ParameterKey=InstanceType,ParameterValue=t2.micro ParameterKey=KeyName,ParameterValue=mykey-s ParameterKey=ServicePort,ParameterValue=8080 ParameterKey=DBName,ParameterValue=myapp ParameterKey=DBUserName,ParameterValue=myapp ParameterKey=DBUserPassword,ParameterValue=myapp12345
