# 🧩 Job Market Analytics Pipeline

## 📖 Overview
**Job Market Analytics Pipeline** is an end-to-end data engineering and analytics project that transforms raw, unstructured recruitment data into a clean, relational **MySQL database**, and visualizes job market insights through **Power BI** dashboards.  

This project helps recruitment firms and analysts explore hiring trends, job types, and in-demand skills across industries — turning messy data into meaningful intelligence.

---

## 🎯 Project Objectives
- 🔹 Consolidate fragmented job datasets into a single, structured database  
- 🔹 Automate data cleaning, transformation, and schema standardization  
- 🔹 Create interactive Power BI dashboards for actionable insights  
- 🔹 Optimize for performance to handle 700K+ records efficiently  

---

## 🧱 Database Schema
| Column Name | Description |
|--------------|-------------|
| `Job_id` | Unique identifier for each job posting |
| `Job_title` | Title or designation of the job |
| `Job_field` | Functional area (e.g., Data Science, Data Engineering) |
| `Company_name` | Name of the hiring organization |
| `Job_location` | City / State / Remote |
| `Job_posting_date` | Date when the job was first posted |
| `Job_level` | Experience level (Entry / Mid / Senior) |
| `Job_type` | Work mode (On-site / Hybrid / Remote) |
| `Job_skills` | Required or preferred technical skills |
| `Job_employment_type` | Employment nature (Permanent / Contract / Internship etc.) |
| `Summary` | Short description or responsibilities |

---

## ⚙️ Tech Stack
| Layer | Tools / Technologies |
|--------|----------------------|
| **Data Processing** | Python (Pandas, NumPy) |
| **Database** | MySQL |
| **ETL & Integration** | PyODBC / MySQL Connector |
| **Visualization** | Power BI (M Language + DAX) |
| **Performance Handling** | Chunk-based data ingestion |

---

## 🧹 Data Transformation Highlights
<details>
<summary>🔧 Expand to view details</summary>

- 🧩 **Normalization** — Merged and aligned multiple data sources under one schema  
- 🧼 **Cleaning** — Removed duplicates, nulls, and invalid records  
- 🧠 **Categorization (Power BI M-Code)**  
  - Derived `Job_employment_type` from keywords like *full-time*, *contract*, *internship*, etc.  
  - Classified `Job_title` into consistent categories (e.g., *Data Analyst*, *Cloud Engineer*, *Software Engineer*) using Power Query conditional logic  
- ⚙️ **Optimization** — Chunk-based inserts to handle >700,000 rows efficiently in Python  

</details>

---

## 📊 Power BI Visualizations
<details>
<summary>📈 Click to expand the list of dashboards</summary>

1. **Hiring Trends Over Time** → Job postings per year for trend analysis  
2. **Distribution of Job Types** → Breakdown of remote, hybrid, and on-site roles  
3. **Top Job Types per Country & Year** → Regional hiring insights  
4. **Average Number of Companies Hiring Over Time** → Measures market activity  
5. **Top 3 Job Fields by Year** → Identifies high-demand sectors annually  
6. **Most In-Demand Skills** → Visual representation of skill frequency  

</details>

---

## 🚀 Key Features
- 💾 Handles datasets with 700K+ records effortlessly  
- 🧮 Automated ETL from CSV → MySQL → Power BI  
- 🧱 Clean mapping between relational schema and Power BI visuals  
- ⚡ Optimized report performance with efficient data modeling  

---

## 📁 Folder Structure
```bash
job-market-analytics-pipeline/
│
├── data2/ # 📊 Raw job data files (CSV)
├── project objectives/ # 🎯 Problem statement files (PDF)
├── transformation/ # ⚙️ DAX, M-code transformations & Python ETL scripts
├── visualization/ # 📈 Power BI (.pbix) dashboards
└── README.md # 📝 Project overview (this file)
