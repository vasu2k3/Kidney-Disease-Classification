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

MLFLOW_TRACKING_URI=https://dagshub.com/vasanth.vasu2002/Kidney-Disease-Classification.mlflow
MLFLOW_TRACKING_USERNAME=vasanth.vasu2002
MLFLOW_TRACKING_PASSWORD=665abe144f104cd8c3a6dbf6ee7164c6c7fedb98
python script.py
```bash
export MLFLOW_TRACKING_URL=https://dagshub.com/vasanth.vasu2002/Kidney-Disease-Classification.mlflow
```
```bash
export MLFLOW_TRACKING_USERNAME=vasanth.vasu2002
```
```bash
export MLFLOW_TRACKING_PASSWORD=665abe144f104cd8c3a6dbf6ee7164c6c7fedb98
```


