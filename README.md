# Scalable Machine Learning Opearations (MLOps)

## MLOps maturity level 5 

## Overview :
This project focuses on building a robust and scalable MLOps pipeline to automate the machine learning lifecycle, including model integration, deployment, monitoring, and maintenance. By leveraging AWS, Kubernetes, and open-source technologies, the solution ensures efficient, reproducible, and reliable workflows while supporting continuous delivery and operational scalability.

## Key Features :

**Data Versioning** : DVC

**Continuous Integration(CI)** : Triggered through ‘main.yml’ , building the code (docker), tests the code(Pytest),pushes the docker image to AWS ECR. 

**Experiment Tracking / Model Versioning** : MLflow 

**Continuous Deployment(CD)** : Deploys FastAPI in AWS EKS(kubernetes cluster) for real-time and batch predictions. 

**Continuous Monitoring(CM)** : Integrating the ‘/metrics’ method of  FastAPI in Prometheus and visualizes endpoints in Grafana.  

**Continuous Training(CT)** : Triggers code execution through GitHub Actions when new data is pushed to the remote DVC location and committed to Git. 

**Drift Monitoring** : Uses a Streamlit app to monitor data drift, target drift, and performs data quality checks.

