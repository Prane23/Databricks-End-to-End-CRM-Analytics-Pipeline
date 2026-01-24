# ![Databricks](https://img.shields.io/badge/Platform-Databricks-orange?logo=databricks) Databricks End-to-End CRM Analytics Pipeline

This project demonstrates an end-to-end Customer Relationship Management (CRM) analytics pipeline built on Databricks. It covers the entire lifecycle of data processing, from ingestion to visualization, leveraging Apache Spark, Delta Lake, and Databricks notebooks for scalable and efficient analytics.
The pipeline is designed to:

Ingest raw CRM data from csv file.
- Perform data cleaning, transformation, and enrichment.
- Store processed data in Delta tables for reliability and performance.
- Generate actionable insights through advanced analytics and visualization.

## ✅ Features
-  Data Ingestion: Load raw CRM data from CSV/Parquet file or external sources.
-  Data Transformation: Apply Spark-based transformations for cleaning and feature engineering.
-  Delta Lake Integration: Ensure ACID transactions and versioning for data reliability.
-  Analytics & Visualization: Build dashboards and reports for customer segmentation, churn prediction, and revenue analysis.
-  Scalable Architecture: Designed for large-scale CRM datasets using Databricks clusters.
---
## 🛠 Tech Stack
- Databricks
- Apache Spark
- PySpark
- Delta Lake
- Databricks SQL
---
## 🏗️ Architecture
The pipeline consists of the following stages:
1. Raw Data Layer
   - Source: CRM system exports (CSV)
   - Storage: Databricks File System (DBFS)
2. Bronze Layer
   - Raw ingestion into Delta tables.
3. Silver Layer
   - Data cleaning and transformation (handling nulls, duplicates, normalization).
4. Gold Layer
   - Aggregated and enriched data for analytics and reporting.
5. Visualization
   - Dashboards using Databricks SQL or integration with BI tools (Power BI/Tableau).

---
## 🔄 Workflow

- Upload raw sales data to Bronze.
- Clean and transform in Silver.
- Aggregate for analytics in Gold.
- Validate outputs using Databricks SQL.
---
🚀 Getting Started

Clone the Repository
git clone https://github.com/Prane23/Databricks-End-to-End-CRM-Analytics-Pipeline.git

- 1 Import Notebooks into your Databricks workspace.
- 2 Configure/run cluster 
- 3 Run ETL Pipeline:
  - Bronze: Raw data ingestion
  - Silver: Data cleansing
  - Gold: Analytics-ready tables
- 4 Schedule Jobs using /jobs configs.
---
## 📂 Folder Structure
```
project-root/
│
├── Initialize_lakehouse/          # Initialize_lakehouse script Initialze_lakehouse.ipynb
├── bronze/                        # bronze layer bronze_layer.ipynb script
├── silver/                        # silver layer silver.ipynb script
├── gold/                          # gold layer gold.ipynb script
├── data/                          # sales raw data (csv file)
├── jobs/                          # 
├── .databricks/                   # Internal Databricks metadata
└── README.md                      # Project overview
```

## 🔗 Configure Git Integration in Databricks
To keep your notebooks and scripts version-controlled and synced with GitHub:

Enable Git Integration in Databricks:

- Go to workspace → create git folder
- Select Git Provider (e.g., GitHub).
- Generate a Personal Access Token from GitHub and paste it in Databricks.

<img width="1200" height="563" alt="image" src="https://github.com/user-attachments/assets/6c9ca1dd-53ca-448e-a53b-dab12f0ace76" />

In Databricks, open a notebook.
- Add a commit message and push directly to GitHub.
- Best Practice:
   - se feature branches for development.
   - Regularly sync changes to avoid conflicts.
---
## 🔗 Create and schedule the job using databrick 
<img width="1611" height="1047" alt="image" src="https://github.com/user-attachments/assets/18e06985-29e8-46b0-9ee1-89cace8887ef" />

## 🔗 Monitor and check the status of the job
<img width="1615" height="947" alt="image" src="https://github.com/user-attachments/assets/ca1f0cd9-e45c-4823-a831-5fbcf2f3691a" />

<img width="1400" height="951" alt="image" src="https://github.com/user-attachments/assets/b90ea7bb-0c4b-45ac-ba35-0b356179ec7e" />

## 📊 Create visualization using databrick dashboard 
<img width="1716" height="919" alt="image" src="https://github.com/user-attachments/assets/3ff6cb2d-be27-4f03-a5cc-1ccf577d7ae9" />

---
## 🌟 Future Enhancements
- Add data quality monitoring.
- Implement Slowly Changing Dimensions (SCD).

