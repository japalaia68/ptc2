# Plan A DevOps Challenge 2

## Task
1. Create code for deploying a VPC in AWS with 2 public and 2 private subnets.

Clone Repo

Run:

`aws cloudformation --region us-east-1 create-stack --stack-name <name stack> --template-body file://DeployVPC.yaml
`
2. Create code for deploying an EKS cluster in AWS, which will use the VPC created in the previous step. The cluster must have 2 nodes, using instance type t3a.large. The nodes must be on the private subnets only.

Clone Repo

This code will create the vpc resources and what is requested at this point

Delete previously created resources.

`aws cloudformation --region us-east-1 delete-stack --stack-name <name stack>
`
Run:

`aws cloudformation --region us-east-1 create-stack --stack-name <name stack> --template-body file://AWSFULL.yaml --capabilities CAPABILITY_NAMED_IAM`