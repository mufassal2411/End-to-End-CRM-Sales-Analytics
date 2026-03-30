# 📊 End-to-End CRM Sales Analytics Pipeline

## 🚀 Project Overview

This project demonstrates an **end-to-end data engineering and analytics pipeline** built using Python, PostgreSQL, and Power BI.

The goal was to transform raw CRM sales data into a structured format, perform analysis, and create an interactive dashboard to generate business insights.

---

## 🧠 Objectives

* Clean and preprocess raw CRM data
* Design a structured data model (Star Schema)
* Build an ETL pipeline using Python
* Store data in PostgreSQL
* Perform SQL-based analysis
* Create an interactive Power BI dashboard

---

## 🧱 Architecture

**Flow:**
CSV Files → Python (ETL) → PostgreSQL → Power BI Dashboard

---

## 🛠️ Tech Stack

* **Python (pandas)** → Data cleaning & transformation
* **PostgreSQL** → Data storage
* **SQL** → Data analysis
* **Power BI** → Data visualization

---

## 📂 Dataset

The dataset consists of CRM sales-related tables:

* Accounts
* Products
* Sales Team
* Sales Pipeline

---

## 🔄 ETL Process

### 1. Extract

* Loaded raw CSV files into Python using pandas

### 2. Transform

* Cleaned column names and data types
* Converted date fields to datetime
* Handled missing values and inconsistencies
* Standardized text data (lowercase, trimmed spaces)
* Created dimension tables:

  * dim_accounts
  * dim_products
  * dim_sales_team
* Generated surrogate keys (IDs)
* Built a fact table: `fact_sales_pipeline`

### 3. Load

* Loaded transformed data into PostgreSQL using SQLAlchemy

---

## ⭐ Data Modeling (Star Schema)

* **Fact Table**

  * fact_sales_pipeline

* **Dimension Tables**

  * dim_accounts
  * dim_products
  * dim_sales_team

This design improves query performance and ensures scalability.

---

## 📊 SQL Analysis

Key queries performed:

* Total revenue calculation
* Revenue by product
* Sales agent performance
* Monthly revenue trends
* Conversion rate calculation
* Running totals using window functions

---

## 📈 Power BI Dashboard

### Features:

* KPI Cards:

  * Total Revenue
  * Total Deals
  * Conversion Rate
  * Average Deal Size
* Revenue trend over time
* Sales agent performance
* Top products analysis
* Top customers
* Deal stage distribution
* Interactive slicers (filters)

---

## 🔍 Key Insights

* Conversion rate is approximately 48%, indicating moderate sales efficiency
* A few sales agents contribute the majority of revenue
* Revenue shows fluctuations across months
* Top products and customers drive significant business value

---

## 💡 Learnings

* Hands-on experience with ETL pipelines
* Understanding of data modeling (star schema)
* Writing analytical SQL queries
* Building interactive dashboards
* End-to-end data workflow integration

---

## 📌 Future Improvements

* Automate ETL pipeline scheduling
* Add more advanced SQL analytics
* Integrate real-time data sources
* Enhance dashboard UI/UX

---

## 👨‍💻 Author

**Mufassal M Areeb**

---

## ⭐ Conclusion

This project demonstrates the ability to build a complete **data pipeline from raw data to business insights**, showcasing both data engineering and data analytics skills.
