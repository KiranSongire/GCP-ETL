--ETL Pipeline on Google Cloud Platform--

--Introduction

This project implements an ETL pipeline for processing audible transaction data and book metadata using Google Cloud Platform (GCP). The workflow is managed with Apache Airflow (via Cloud Composer) to extract, transform, and load data into a data lake and BigQuery for analysis and visualization.

--Tools Used
Cloud Storage: Data lake for raw and processed data.
Google Colab: Data cleansing and preprocessing.
Cloud Composer: Workflow orchestration with Apache Airflow.
BigQuery: Data warehouse for querying and analysis.
Data Studio: Visualization and reporting.

--Pipeline Workflow
Extract:

Fetched transaction data from MySQL and metadata from a REST API.
Saved raw data to Cloud Storage.
Transform:

Cleaned and merged datasets using Python scripts.
Load:

Stored processed data in Cloud Storage.
Load specific tables into BigQuery for analysis.
Visualize:

Used Google Data Studio to create dashboards and insights.


--Outputs
Cloud Storage: Processed data stored in buckets.
BigQuery: Datasets and tables ready for querying.
Data Studio: Interactive dashboards for analysis.