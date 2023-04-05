# VERSION 2.5.3
# AUTHOR: Anuj and Kumarswami
# DESCRIPTION: Basic Airflow container
# BUILD: docker build --rm -t airflow .
# SOURCE: https://github.com/
FROM apache/airflow:2.5.3
ARG AIRFLOW_UID=501
ARG AIRFLOW_GID=0 

LABEL maintainer="anuj_kumar"
ENV DEBIAN_FRONTEND noninteractive
USER root
RUN apt-get update
RUN apt-get -y install gcc 
RUN rm -rf /var/lib/apt/lists/*
USER airflow
RUN pip install -U pip
RUN pip install -U pyOpenSSL 
RUN pip install pyasn1 
RUN pip install requests 
RUN pip install pandas  
# RUN pip install pymongo  
RUN pip install numpy 
RUN pip install lxml 
RUN pip install oracledb 
RUN pip install ibm-db 
RUN pip install pymssql 
RUN pip install psycopg 
RUN pip install apache-airflow-providers-apache-spark 
RUN pip install apache-airflow-providers-cncf-kubernetes 
RUN pip install apache-airflow-providers-common-sql 
RUN pip install apache-airflow-providers-databricks 
RUN pip install apache-airflow-providers-jdbc 
RUN pip install apache-airflow-providers-microsoft-mssql 
RUN pip install apache-airflow-providers-mysql 
RUN pip install apache-airflow-providers-odbc 
RUN pip install apache-airflow-providers-oracle 
RUN pip install apache-airflow-providers-postgres 