FROM continuumio/miniconda3:latest

RUN pip install mlflow boto3 pymysql

ADD . /app
WORKDIR /app

COPY . .

SHELL [ "bin/bash", "-c" ]

RUN chmod +x wait-for-it.sh

