# Classification-Model

## Workflows

Update config.yaml
Update secrets.yaml [Optional]
Update params.yaml
Update the entity
Update the configuration manager in src config
Update the components
Update the pipeline
Update the main.py
Update the dvc.yaml


# How to run?
# STEPS:
Clone the repository

https://github.com/Kornadevika/Classification-Model.git

# STEP 01- Create a conda environment sfter opening repository

conda create -n Classification-Model python=3.8 -y
conda activate Classification-Model

# STEP -2- install the requirements

pip install -r requiremnts.txt

# Finally run the following command

python app.py

Now,

open up your local host and port

# DVC cmd

1.dvc init
2.dvc repro
3.dvc dag

# AWS-CICD-Deployment-with-Github-Actions

1.Logib to AWS console
2.Create IAM user for deployment

#with specific access

1. EC2 access : It is virtual machine

2. ECR: Elastic Container registry to save your docker image in aws


#Description: About the deployment

1. Build docker image of the source code

2. Push your docker image to ECR

3. Launch Your EC2 

4. Pull Your image from ECR in EC2

5. Lauch your docker image in EC2

#Policy:

1. AmazonEC2ContainerRegistryFullAccess

2. AmazonEC2FullAccess

3.Create ECR repo to store/save docker image
-save the Url: 361769587084.dkr.ecr.us-east-1.amazonaws.com/deeplearning

# 4. Create EC2 machine (Ubuntu)
# 5. Open EC2 and install docker in EC2 Machine:

#optinal

sudo apt-get update -y

sudo apt-get upgrade

#required

curl -fsSL https://get.docker.com -o get-docker.sh

sudo sh get-docker.sh

sudo usermod -aG docker ubuntu

newgrp docker

# 6. Configure EC2 as self-hosted runner:

setting>actions>runner>new self hosted runner> choose os> then run command one by one

# 7. Setup github secrets:
AWS_ACCESS_KEY_ID=

AWS_SECRET_ACCESS_KEY=

AWS_REGION = us-east-1

AWS_ECR_LOGIN_URI = 

ECR_REPOSITORY_NAME = 

