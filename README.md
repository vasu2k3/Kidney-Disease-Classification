# Kidney-Disease-Classification

## Workflows

1. Update config.yaml
2. Update secrets.yaml [Optional]
3. Update params.yaml
4. Update the entity
5. Update the configuration manager in src config
6. Update the components
7. Update the pipeline 
8. Update the main.py
9. Update the dvc.yaml
10. app.py

# How to run?
### STEPS:

### Clone the repository
```bash
git clone https://github.com/vasu2k3/Kidney-Disease-Classification
```
### STEP 01- Create a conda environment after opening the repository
```bash
conda create -n kidney python=3.9 -y
```
```bash
conda activate kidney
```

### STEP 02- install the requirements
```bash
pip install -r requirements.txt
```

# MLflow
dagshub
-used for evaluating the model
```bash
import dagshub
dagshub.init(repo_owner='vasanth.vasu2002', repo_name='Kidney-Disease-Classification', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)
```
## DVC Commands
-used for not repeating the same unnecessary steps in pipeline 
```bash 
dvc init
```
```bash
dvc repro
```
```bash
dvc dag
```

# AWS CI/CD Deployment

## 1. Login to AWS console.

## 2. Create IAM user for deployment

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

	
