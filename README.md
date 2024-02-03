# Realtime Data Streaming | End-to-End Data Engineering Project

## Table of Contents

- [Realtime Data Streaming | End-to-End Data Engineering Project](#realtime-data-streaming--end-to-end-data-engineering-project)
  - [Table of Contents](#table-of-contents)
  - [Introduction](#introduction)
  - [System Architecture](#system-architecture)
  - [What You'll Learn](#what-youll-learn)
  - [Technologies](#technologies)
  - [Getting Started](#getting-started)

## Introduction

This project constitutes a comprehensive guide delineating the development of a holistic data engineering pipeline. It meticulously traverses every stage of the process, commencing from data ingestion, progressing through processing, and culminating in storage. This endeavor leverages a resilient technological stack encompassing prominent tools such as Apache Airflow, Python, Apache Kafka, Apache Zookeeper, Apache Spark, and Cassandra. To ensure seamless deployment and scalability, all components are encapsulated within Docker containers, thereby streamlining operations and enhancing adaptability to varying workloads.

## System Architecture

![System Architecture]()

The project is designed with the following components:

- **Data Source**: We use `randomuser.me` API to generate random user data for our pipeline.
- **Apache Airflow**: Responsible for orchestrating the pipeline and storing fetched data in a PostgreSQL database.
- **Apache Kafka and Zookeeper**: Used for streaming data from PostgreSQL to the processing engine.
- **Control Center and Schema Registry**: Helps in monitoring and schema management of our Kafka streams.
- **Apache Spark**: For data processing with its master and worker nodes.
- **Cassandra**: Where the processed data will be stored.

## What You'll Learn

1. Establishing a Data Pipeline Utilizing Apache Airflow
2. Implementing Real-Time Data Streaming Using Apache Kafka
3. Orchestrating Distributed Synchronization via Apache Zookeeper
4. Employing Advanced Data Processing Techniques with Apache Spark
5. Leveraging Efficient Data Storage Solutions Provided by Cassandra and PostgreSQL
6. Containerization of the Entire Data Engineering Infrastructure with Docker

## Technologies

- Apache Airflow
- Python
- Apache Kafka
- Apache Zookeeper
- Apache Spark
- Cassandra
- PostgreSQL
- Docker

## Getting Started

1. Clone the repository:

   ```bash
   git clone https://github.com/BrC-Habeda/data-engineering.git
   ```

2. Navigate to the project directory:

   ```bash
   cd data-engineering
   ```

3. Run Docker Compose to spin up the services:
   ```bash
   docker-compose up
   ```
