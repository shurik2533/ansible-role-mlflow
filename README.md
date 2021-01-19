# Ansible Role: MLflow
Ansible playbook for [MLflow](https://www.mlflow.org/)

Creates docker container with MLflow. 

PostgreSQL used as backend-store. Minio used for artifact storage.

Minio and PostgreSQL are also installed in separate docker containers

# Run MLflow on localhost example
`ansible-playbook main.yml`

MLflow will be at http://localhost:5000
