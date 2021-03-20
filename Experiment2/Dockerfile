FROM python:3-slim

RUN pip3 install mlflow
RUN mkdir -p /srv/mlflow

EXPOSE 5000

CMD ["mlflow", "server", "--backend-store-uri", "sqlite:///mlflow.db", "--host", "0.0.0.0", "--default-artifact-root", "file:/mlflow"]

