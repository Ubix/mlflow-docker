FROM continuumio/miniconda3:latest

RUN pip install mlflow boto3 pymysql

ADD . /app
WORKDIR /app

COPY . .
RUN ["/bin/bash", "-c", "chmod +x wait-for-it.sh"]

