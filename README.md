# MLFlowBasic-Operation



## For Dagshub: Add to example.py


'''bash

MLFLOW_TRACKING_URL=https://dagshub.com/Tomisin92/MLFlowBasic-Operation.mlflow

import dagshub
dagshub.init(repo_owner='Tomisin92', repo_name='MLFlowBasic-Operation', mlflow=True)


## MLflow on AWS Setup
1. Login to AWS console
2. Create IAM user for deployment
3. Export the credentials in your AWS CLI by running "aws configure'
4. Create a s3 bucket
5. Create EC2  MACHINE (Ubuntu) & add security group 5000 port

## with specific access

1. EC2 access : It is virtual machine

2. ECR: Elastic Container registry to save your docker image in aws


## Description: About the deployment

1. Build docker image of the source code

2. Push your docker image to ECR

3. Launch Your EC2 

4. Pull Your image from ECR in EC2

5. Lauch your docker image in EC2

## Policy:

1. AmazonEC2ContainerRegistryFullAccess

2. AmazonEC2FullAccess