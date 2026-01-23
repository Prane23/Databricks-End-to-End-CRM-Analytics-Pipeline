# ![Databricks](https://img.shields.io/badge/Platform-Databricks-orange?logo=databricks) Databricks End-to-End CRM Analytics Pipeline

This project demonstrates an end-to-end data pipeline for CRM analytics using Databricks. It covers ingestion, transformation, and analytics layers following the Medallion Architecture (Bronze → Silver → Gold).
The pipeline is designed to:
   -  Ingest raw CRM data from multiple sources.
   -  Cleanse and standardize data for analytics.
   -  Generate curated datasets for reporting and insights.
---
## 🛠 Tech Stack
- Databricks
- PySpark
- Delta Lake
- Databricks SQL
---
## 🏗 Architecture
Sales Data → Bronze → Silver → Gold
- Bronze: Raw sales data
- Silver: Cleaned and standardized data
- Gold: Aggregated data for business insights

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
---
## 🌟 Future Enhancements

- Add data quality monitoring.
- Implement Slowly Changing Dimensions (SCD).
- Integrate BI tools for visualization.
