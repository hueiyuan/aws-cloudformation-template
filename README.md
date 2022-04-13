# aws-cloudformation-template
the repo includes my experience about aws cloudformation yaml. If need it, we have to replace value for our real situation.

## All services
1. AWS MSK
2. AWS EMR
3. AWS Redsfhit
4. AWS ALB
5. Redash Dashboard Service
6. Kafka UI Service
7. Schema Registry Service

## Related AWS Cloudformation cli example 
* Create Cloudformation Stack
```
aws cloudformation create-stack --stack-name {your-stack-name} --capabilities CAPABILITY_NAMED_IAM --template-body file://{cf-yaml-file-path} --tags Key={key1},Value={val1} Key={key2},Value={val2}
```

* Validate Cloudformation Stack
```
aws cloudformation validate-template --template-body file://{cf-yaml-file-path}
```

* Update Cloudformation Stack
```
aws cloudformation update-stack --stack-name {your-stack-name} --capabilities CAPABILITY_NAMED_IAM --template-body file://{cf-yaml-file-path}
```

* Delete Cloudformation Stack
```
aws cloudformation delete-stack --stack-name {your-stack-name}
```

## Reference
* [AWS ClI Reference on Cloudformation](https://docs.aws.amazon.com/cli/latest/reference/cloudformation/index.html#cli-aws-cloudformation)
* [AWS Cloudformation Documentation](https://docs.aws.amazon.com/cloudformation/)
