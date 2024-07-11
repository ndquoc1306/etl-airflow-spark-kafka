# Realtime Data Streaming | End-to-End Data Engineering Project

## Table of Contents
- [Introduction](#introduction)
- [System Architecture](#system-architecture)
- [Describe Project](#describe-project)
- [Technologies](#technologies)
- [Getting Started](#getting-started)

## Introduction

This project serves as a comprehensive guide to building an end-to-end data engineering pipeline. It covers each stage from data ingestion to processing and finally to storage, utilizing a robust tech stack that includes Apache Airflow, Python, Apache Kafka, Apache Zookeeper, Apache Spark, and Cassandra. Everything is containerized using Docker for ease of deployment and scalability.

## System Architecture

![architecture.png](architecture.png)

The project is designed with the following components:

- **Data Source**: We use `randomuser.me` API to generate random user data for our pipeline.
- **Apache Airflow**: Responsible for orchestrating the pipeline and storing fetched data in a PostgreSQL database.
- **Apache Kafka and Zookeeper**: Used for streaming data from PostgreSQL to the processing engine.
- **Control Center and Schema Registry**: Helps in monitoring and schema management of our Kafka streams.
- **Apache Spark**: For data processing with its master and worker nodes.
- **Cassandra**: Where the processed data will be stored.

## Describe Project

- Setting up a data pipeline with Apache Airflow
- Real-time data streaming with Apache Kafka
- Distributed synchronization with Apache Zookeeper
- Data processing techniques with Apache Spark
- Data storage solutions with Cassandra and PostgreSQL
- Containerizing your entire data engineering setup with Docker

## Technologies

- Apache Airflow: Open-source tool for scheduling and monitoring workflows.
- Python: High-level programming language known for its simplicity and versatility.
- Apache Kafka: Distributed system for high-throughput data streaming.
- Apache Spark: Engine for processing large datasets, supports streaming, SQL, ML, and graph tasks.
- Cassandra: NoSQL DB for large-scale, fault-tolerant data storage.
- PostgreSQL: pen-source relational DB emphasizing extensibility and SQL standards.
- Docker: Tool for creating consistent and isolated application containers.

## Getting Started

1. Clone the repository:
    ```bash
    git clone https://github.com/ndquoc1306/etl-airflow-spark-kafka.git
    ```

2. Navigate to the project directory:
    ```bash
    cd etl-airflow-spark-kafka
    ```

3. Run Docker Compose to spin up the services:
    ```bash
    docker-compose up
    ```