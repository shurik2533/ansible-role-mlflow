FROM python:3.7.0
RUN mkdir /mlflow/
RUN pip install mlflow psycopg2 boto3

CMD mlflow server \
--backend-store-uri postgresql://${POSTGRES_USER}:${POSTGRES_PASSWORD}@${DOCKER_HOST}:${POSTGRES_PORT}/${DB_NAME} \
--host 0.0.0.0 \
--port ${MLFLOW_PORT} \
--default-artifact-root s3://${MLFLOW_S3_BUCKET}
