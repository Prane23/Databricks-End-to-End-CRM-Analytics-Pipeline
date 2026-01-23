# 🚀 Databricks End-to-End CRM Analytics Pipeline
 An end-to-end pipeline on Databricks using PySpark and Delta Lake to process sales data into Bronze, Silver, and Gold layers following the Medallion Architecture for analytics and reporting.

🛠 Tech Stack
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

## 📂 Folder Structure
├
├── README.md
---

## 🌟 Future Enhancements

- Add data quality monitoring.
- Implement Slowly Changing Dimensions (SCD).
- Integrate BI tools for visualization.
