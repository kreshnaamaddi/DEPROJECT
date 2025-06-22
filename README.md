
## 🔷 Azure Data Engineering Project – Real-Time Pipeline using Medallion Architecture

This project demonstrates a **complete end-to-end Azure Data Engineering solution** using real-time data, built to reflect real-world enterprise architecture and practices. It is designed to help professionals prepare for Azure Data Engineering roles by showcasing hands-on experience with in-demand tools and technologies.

---

### 🏗️ Architecture: **Medallion Architecture (Bronze, Silver, Gold)**

We followed the Medallion Architecture to organize and process data in a structured, scalable, and modular manner:

* **Bronze Layer** – Stores raw data as-ingested from the source.
* **Silver Layer** – Contains cleaned and transformed data.
* **Gold Layer** – Optimized data ready for analytics and reporting.

---

### ⚙️ Tools & Technologies Used:

| Tool                               | Purpose                                     |
| ---------------------------------- | ------------------------------------------- |
| **Azure Data Factory (ADF)**       | Data ingestion from REST API                |
| **Azure Data Lake Storage (ADLS)** | Layered data storage (Bronze, Silver, Gold) |
| **Azure Databricks (PySpark)**     | Data transformation and processing          |
| **Azure Synapse Analytics**        | Data warehousing and SQL-based analytics    |
| **Power BI**                       | Data visualization and dashboarding         |
| **GitHub REST API**                | Real-time JSON data source                  |

---

### 🔁 Project Workflow:

1. **Data Ingestion (ADF + REST API):**

   * Azure Data Factory fetches live data from the **GitHub REST API**.
   * Data is stored in **JSON format** in the **Bronze layer** of Azure Data Lake.

2. **Data Transformation (Databricks - PySpark):**

   * Databricks notebooks read the Bronze data using PySpark.
   * Data cleaning, parsing, normalization, and schema enforcement are applied.
   * Cleaned data is written to the **Silver layer** of ADLS.

3. **Data Loading (Azure Synapse Analytics):**

   * Transformed data from the Silver layer is ingested into **Synapse dedicated SQL pools**.
   * SQL queries enable analytical insights, joins, and aggregations.

4. **Reporting (Power BI):**

   * Synapse is connected to Power BI for visualization.
   * Built interactive dashboards showing curated data for decision-making.

---

### 🔐 Additional Features:

* **Dynamic Pipelines in ADF:**
  Used parameters and expressions in ADF pipelines to make them reusable and scalable for different datasets or environments.

* **Managed Identity Authentication:**
  Enabled secure communication between ADF, ADLS, and Databricks without using keys or secrets.

* **Error Handling & Logging:**
  Implemented basic logging for monitoring pipeline status and failures.

---

### 📌 Highlights:

* Real-time data pipeline with GitHub as the source.
* Covers essential Data Engineering tools in the Azure ecosystem.
* Follows best practices with layered architecture and secure access.
* Suitable for interviews and portfolio showcasing.
* Scalable for adding more sources or destinations.

---

### 📊 Sample Output:

| Layer  | Sample Data Format                 |
| ------ | ---------------------------------- |
| Bronze | Raw JSON from GitHub               |
| Silver | Structured & cleaned Parquet files |
| Gold   | SQL tables in Synapse Analytics    |

---


