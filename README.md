# Azure-DevOps-Olympic-Podium
Olympic Data Analytics | Azure End-To-End Data Engineering Project


This project focuses on performing an **ETL pipeline and dashboarding** on the **Tokyo Olympics dataset** using Microsoft Azure cloud services.

---

## Project Overview

The project is divided into two major parts:
1. **ETL of Tokyo Olympic data and analytical querying**
2. **Dashboarding using Tableau**

---

## Data Source

- GitHub is used as the **primary source** of the raw dataset (`CSV` format).

---

## ☁Azure Services Explored

### Azure Data Factory (ADF)
- Used to build a data pipeline.
- Integrates and extracts data from GitHub.

### Azure Data Lake Gen2
- Object storage for structured and unstructured data.
- Stores raw and transformed datasets.

### Azure Databricks
- Analytics platform using **Apache Spark**.
- Transforms raw data using **PySpark**.

### Azure Synapse Analytics
- Cloud SQL Data Warehouse.
- Enables advanced querying and analysis.

---

## ETL Workflow

1. **Extract** raw data from GitHub using ADF Pipeline.
2. **Store** raw data in Azure Data Lake.
3. **Transform** the data using PySpark in Azure Databricks.
4. **Store transformed** data back in Azure Data Lake.
5. **Load** the data into target tables in Azure Synapse Analytics.
6. **Analyze** the data using SQL queries.

---

## Dashboarding in Tableau

1. Extract the raw CSV file using ADF Pipeline into Azure Synapse Analytics.
2. Pipeline converts the data into **Parquet** format and stores it back in the Data Lake.
3. Spark database is created, pointing to the Parquet file.
4. Query Spark table using **serverless SQL**.
5. **Tableau** connects to serverless SQL and visualizes data through interactive graphs.

---

## Project Architecture

![Azure-Olympic-ETL-Diagram](assets/olympic-azure-architecture.png)

> 💡 *Place your diagram image in a folder named `assets` inside your repo and name it `olympic-azure-architecture.png`, or update the path above accordingly.*

---

## Folder Structure

Azure-DevOps-Olympic-Podium/
│
├── assets/
│ └── olympic-azure-architecture.png
├── data/
│ └── olympic_raw_data.csv
├── notebooks/
│ └── transform_data_pyspark.ipynb
├── pipeline/
│ └── adf_pipeline.json
├── queries/
│ └── synapse_queries.sql
└── README.md


---

## Status

✔️ ETL Pipeline Completed  
✔️ Tableau Dashboard Integrated  
✔️ Azure Service Workflow Functional

---



