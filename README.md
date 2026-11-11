
# 🏏 Cricket Data Engineering Pipeline

An end-to-end Big Data Engineering project that ingests cricket match data through an external API, processes it using Apache Spark, and transforms raw data into structured datasets for analytical insights.

The project implements the **Medallion Architecture (Bronze, Silver and Gold)** to demonstrate a structured data engineering workflow.

## 📌 Project Overview

This project focuses on building a data pipeline using cricket match data obtained through the CricAPI. The pipeline covers API ingestion, raw data storage, data cleaning, transformation, and preparation of analytical datasets.

The objective is to convert raw cricket data into meaningful, analysis-ready information using modern data engineering tools and techniques.

## 🏗️ Architecture

The project follows the Medallion Architecture:

### 1. Bronze Layer – Raw Data Ingestion
- Fetches cricket match data using the CricAPI.
- Retrieves live/current match information through API requests.
- Stores the raw API response in JSON format.
- Creates a Spark DataFrame to maintain the ingested data along with source and ingestion timestamp metadata.

### 2. Silver Layer – Data Cleaning & Transformation
- Processes raw data from the Bronze layer.
- Cleans and structures the match data.
- Handles data inconsistencies and prepares structured datasets.
- Creates clean match tables for further analysis.

### 3. Gold Layer – Analytics & Insights
- Transforms cleaned data into analytics-ready datasets.
- Prepares aggregated and structured information.
- Enables downstream analysis and generation of meaningful cricket insights.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | API ingestion and data processing |
| CricAPI | Cricket match data source |
| Apache Spark | Distributed data processing |
| PySpark | DataFrame transformations |
| JSON | Raw API response storage |
| SQL | Data querying and analysis |
| Databricks | Development and execution environment |
| Git & GitHub | Version control |

## 🔄 Data Pipeline Workflow

1. Connect to CricAPI and retrieve cricket match data.
2. Capture and store the raw API response.
3. Ingest the raw data into the Bronze layer.
4. Clean and transform the data into the Silver layer.
5. Prepare analytical datasets in the Gold layer.
6. Use the refined datasets for cricket analytics and insights.

## 📂 Project Structure

```text
Cricket-Data-Engineering-Pipeline/
│
├── 1_API Ingestion and Bronze Layer.py
│
├── 2_BronzetoSilverCleanMatchTable.py
│
├── 3_GoldLayerAnalyticsPrepration.py
│
├── Flow of Project.drawio
│
└── README.md
```

## 🎯 Key Learning Outcomes

- Working with external REST APIs using Python.
- Handling JSON responses and raw data ingestion.
- Understanding the Medallion Architecture.
- Creating and managing PySpark DataFrames.
- Implementing data cleaning and transformation workflows.
- Understanding the fundamentals of building end-to-end data pipelines.
- Preparing structured datasets for analytical use cases.

## 🚀 Future Enhancements

- Automate periodic API ingestion.
- Implement incremental data loading.
- Add data quality checks and validation.
- Integrate visualization tools for cricket analytics.
- Develop dashboards for match-level and player-level insights.


**Built using Python, Apache Spark and the Medallion Architecture.**
