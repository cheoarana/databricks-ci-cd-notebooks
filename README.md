# databricks-ci-cd-notebooks
Repository contains continuous deployment of databricks notebooks
This repository contains a continuous deployment method for Azure Pipelines in Azure DevOps.

## Requirements
The requirements for using this pipeline are as follows:
Create Azure Pipelines libraries with the following names:
* DATABRICKS-TEST
* DATABRICKS-PROD

## Azure Pipeline Library
For ingress, the variables are explained as follows
| Variable | Example                                        |
| -------- | ---------------------------------------------- |
| `DBW-PROFILE` | Databricks cli profile name               |
| `DBW-HOST` | Databricks workspace url |
| `DBW-SECRET` | Databricks workspace administrator user token|
| `REPOSITORY-FOLDERNAME` | Name of the repository folder containing notebooks|
| `NOTEBOOK-PATH` | Path where the notebooks will be deployed|

## Project Structure
```
.
├── databricks-ci-cd-notebooks
│   ├──templates
│   │    └── job-databricks.yml
│   └──azure-pipelines.yaml
└── README.md
```


