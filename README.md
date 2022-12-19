# CloudFormation - Infrastructure As a Code
Infrastructure as a code using CloudFormation example

# What's AWS CloudFormation

AWS CloudFormation is an AWS service that uses template files to automate the setup of AWS resources.

It can also be described as infrastructure automation or Infrastructure-as-Code (IaC) tool and a cloud automation solution because it can automate the setup and deployment of various Infrastructure-as-a-Service (IaaS) offerings on the AWS CloudFormation supports virtually every service that runs in AWS. (A full list of supported services is available here.)

# Steps to create the stack on your AWS account :

## 1- Install AWS CLI

First of all you need to install AWS CLI you can follow the installation guid via the link below : 

    https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html
    
    

## 2- Connect to your aws account

Using your cmd go to the project path and connect to your AWS account using the command `aws-configure` and enter the following information :

  - AWSAccessKeyId
  - AWSSecretKey
  - Region
  - File format (We are using .yaml file format in this example)


## 3- Create your stack

Using the following command in your cmd at your project path to create the stack: 

`aws cloudformation create-stack --stack-name UdgramApp --template-body file://final-project-starter.yml  --parameters file://server-parameters.json --capabilities "CAPABILITY_IAM" "CAPABILITY_NAMED_IAM" --region=us-west-1`
