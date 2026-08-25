# CrimeInsight: Data Engineering and Business Intelligence for Crime Data Analysis

## Project Overview

CrimeInsight is a data engineering and business intelligence project focused on building a structured pipeline for handling crime-related data from multiple sources.

The project is designed to demonstrate how raw crime records can be collected, stored, cleaned, transformed, and prepared for analytical use. It considers both batch data and simulated streaming data to represent different forms of crime-data generation.

The proposed system combines data engineering technologies for ingestion, processing, storage, transformation, orchestration, and visualization. The final analytical layer will support the examination of crime frequency, crime categories, geographic distribution, temporal patterns, and other relevant trends.

The planned technology stack includes Python, PostgreSQL, Apache Kafka, Apache Spark, Apache Airflow, dbt, Power BI, and Docker.

---

## Team Members

| S.No. | Name                   | University ID |
| ----: | ---------------------- | ------------- |
|     1 | Anakala Sarayu         | 2420030249    |
|     2 | Manduri Varshitha      | 2420030269    |
|     3 | Nidumolu Veda Samhitha | 2420030468    |

## Supervisor

**[Supervisor Name]**

---

## Abstract

CrimeInsight is a data engineering and business intelligence system designed to demonstrate the lifecycle of processing and analysing large-scale crime data. The proposed system considers crime records from multiple sources, including CSV files, open datasets, and simulated streaming sources, representing the heterogeneous nature of real-world data.

The system will use Python for crime-data generation and preparation, while Apache Kafka will support streaming ingestion. PostgreSQL will provide structured storage for raw and processed data, and Apache Spark will be used for data validation, cleaning, transformation, and analytical processing. Apache Airflow will coordinate the different stages of the pipeline, while dbt will support analytical transformations and data modelling. Power BI will be used to develop interactive dashboards for examining crime categories, temporal trends, geographic distributions, and other patterns. Docker will provide a consistent environment for the project components.

The project focuses on important data engineering aspects such as data quality, schema consistency, deduplication, normalization, scalable processing, storage, transformation, and workflow orchestration. The resulting analytical datasets will provide a foundation for business intelligence and crime-data analysis.

---

## Objectives

* Build a structured data engineering pipeline for crime-data processing and analysis.
* Collect and prepare crime records from multiple sources, including batch and simulated streaming sources.
* Apply data validation, cleaning, deduplication, and normalization to improve data quality.
* Store and transform crime data into structured datasets suitable for analysis.
* Develop analytical dashboards to identify crime trends, categories, locations, and time-based patterns.

---

## Technology Stack

* **Python** – Crime-data generation, preparation, and supporting data-engineering tasks
* **PostgreSQL** – Structured storage for raw and processed crime data
* **Apache Kafka** – Streaming crime-data ingestion
* **Apache Spark** – Large-scale data processing and transformation
* **Apache Airflow** – Workflow scheduling and pipeline orchestration
* **dbt** – Analytical transformations and data modelling
* **Power BI** – Interactive dashboards and business intelligence
* **Docker** – Containerized and consistent project environment
* **Git & GitHub** – Version control and team collaboration

---

## Proposed Data Flow

The overall system is planned around the following flow:

```text
Crime Data Sources
      |
      +------------------+
      |                  |
   Batch Data       Streaming Data
      |                  |
      |                Kafka
      |                  |
      +--------+---------+
               |
               v
        Raw Data Storage
               |
               v
      Validation & Cleaning
               |
               v
       Spark Processing
               |
               v
      Transformation &
       Data Modelling
               |
               v
      Analytical Storage
               |
               v
          Power BI
               |
               v
      Crime Data Insights

        Airflow
           |
           +--> Coordinates scheduled pipeline tasks
```

The processing stages form part of the same end-to-end pipeline. Data validation, cleaning, processing, transformation, and modelling are connected stages within the overall workflow.

## Current Phase Status

**Current Phase: Post Review 1 – Project Development**

### Completed

* Finalized the CrimeInsight project concept and objectives
* Prepared the project abstract and introduction
* Defined the proposed data engineering architecture
* Selected the initial technology stack
* Completed the Review 1 presentation
* Completed the initial literature survey

### In Progress

* GitHub repository organization
* Project folder and development environment setup
* Planning of crime-data sources and dataset structure

### Planned

* Generate and prepare crime datasets
* Implement batch and streaming ingestion
* Develop the processing and analytical pipeline
* Build the Power BI dashboard and evaluate the results

---

## Repository Structure

```text
CrimeInsight/
│
├── src/
│   └── Project source code
│
├── data/
│   └── Dataset references or project data
│
├── docs/
│   └── Project documentation
│
├── results/
│   └── Processing outputs and generated results
│
├── reports/
│   └── Review presentations and project reports
│
└── README.md
```

Dataset files containing sensitive, restricted, or licensed information will not be committed to the repository. Where required, the corresponding data source or instructions for obtaining the dataset will be documented instead.

---

## Environment Requirements

The planned development environment includes:

* Python 3.x
* PostgreSQL
* Apache Kafka
* Apache Spark
* Apache Airflow
* dbt
* Power BI Desktop
* Docker
* Git

Exact package versions and configuration details will be documented as implementation progresses.

---

## Setup Instructions

### Clone the Repository

```bash
git clone <repository-url>
cd <repository-folder>
```

## Execution Instructions

The intended execution sequence of the project is:

```text
Prepare Crime Data
       ↓
Data Ingestion
       ↓
Raw Data Storage
       ↓
Validation & Cleaning
       ↓
Processing & Transformation
       ↓
Analytical Data
       ↓
Power BI Dashboard
```

Apache Airflow will coordinate the applicable pipeline tasks and scheduled processing activities.

Detailed execution commands will be added as the individual components are implemented.
