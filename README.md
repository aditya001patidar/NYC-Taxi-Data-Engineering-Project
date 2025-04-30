# 🚖NYC-Taxi-Data-Engineering-Project
This project shows how to build a complete data pipeline using Azure tools to turn raw NYC Taxi data into useful insights. The pipeline follows the Medallion Architecture — which means organizing data in three stages:
1) Bronze (Raw)
2) Silver (Cleaned)
3) Gold (Final layer).

## I Use:
- Azure Data Factory to collect data
- Azure Databricks with PySpark to clean and process the data
- Delta Tables to store the final results in a reliable and trackable way

## Working :
### Step 1: Ingest Data with Azure Data Factory (ADF)

- Pulled NYC Taxi data from an external website (API)
- Built ADF pipelines to load data into Azure Data Lake Gen2
- Used folders and subfolders to keep data organized (Hierarchical Namespace)
- This raw data was stored in the Bronze Layer

### Step 2: Transform Data in Azure Databricks

- Used PySpark in Databricks to clean and prepare the data
- Connected securely to Data Lake using Microsoft Entra ID
- Applied cleaning and transformation logic

### Step 3: Store Final Data in Delta Tables
- Saved the cleaned data in Delta Tables in the Gold Layer
- Delta Tables help keep data consistent and safe (ACID compliant)
- Changes to the data are tracked, so we can go back to previous versions if needed

### What I Learned:

- How to build reliable data pipelines using Azure tools
- Hands-on experience with Data Factory, Databricks, Delta Lake, and PySpark
- Learned how to organize data using the Bronze-Silver-Gold model

## Simple Architecture
API (NYC Taxi Data)

      ↓  
Azure Data Factory

      ↓ 
Azure Data Lake Gen2 (Bronze Layer)

      ↓
Azure Databricks + PySpark

      ↓  
Delta Tables (Gold Layer)

## Project Demo

![WhatsApp Image 2025-04-30 at 17 45 56_6ad5f162](https://github.com/user-attachments/assets/6c305b40-8758-4eb6-b1df-aa6d20982224)
