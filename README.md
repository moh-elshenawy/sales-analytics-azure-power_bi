# 🧠 Azure Databricks Power BI Project

## 📋 Overview
This project demonstrates an end-to-end **data engineering pipeline** for analyzing **product sales data** using **Azure Databricks**, **Azure Data Factory**, and **Power BI**.  
The pipeline handles data ingestion from **SQL Server and API**, performs data transformation inside **Databricks**, and visualizes insights through **Power BI dashboards**.

---

## ⚙️ Architecture
The pipeline follows the **Medallion Architecture (Bronze → Silver → Gold)**:

1. **Data Sources**
   - 🧩 **SQL Server:** Main source of transactional product data.  
   - 🌐 **API:** Additional or real-time product/sales information.

2. **Data Ingestion (Azure Data Factory)**
   - ADF extracts data from both **SQL Server** and **API**, and loads it into **Azure Data Lake**.

3. **Data Lake (Storage Account)**
   - Stores the raw (Bronze) and processed (Silver, Gold) data.

4. **Data Processing (Azure Databricks)**
   - Using **PySpark** inside Databricks notebooks to clean, transform, and aggregate the data for analytics.

5. **Data Visualization (Power BI)**
   - Power BI connects to the **Gold layer** and visualizes KPIs and metrics for business insights.

---

## 🧩 Tools & Technologies
- **Azure SQL Server**
- **External REST API**
- **Azure Data Factory**
- **Azure Data Lake (Storage Account)**
- **Azure Databricks (PySpark Notebooks)**
- **Power BI**
- **Python / SQL / JSON**

---

## 🚀 Pipeline Flow
1. Extract data from **SQL Server** and **API** via **Azure Data Factory**  
2. Store raw data in **Azure Data Lake (Bronze)**  
3. Clean and transform in **Azure Databricks (Silver)**  
4. Create analytics-ready data in **Gold Layer**  
5. Connect **Power BI** to the Gold tables and build dashboards  

---

## 📊 Outputs & Visuals

### 🔹 Data Pipeline (Azure Data Factory)


![Pipeline]("C:\Users\yostina\Desktop\project_data\pipline.png")


## 📊 Power BI Dashboard
![Dashboard1]("C:\Users\yostina\Desktop\project_data\dashboard1.jpg")

![Dashboard2]("C:\Users\yostina\Desktop\project_data\dashboard1.jpg")


## 🗂️ Data Flow Example

![Data Flow1]("C:\Users\yostina\Desktop\project_data\data1.png")

![Data Flow2]("C:\Users\yostina\Desktop\project_data\data2.png")

![Data Flow3]("C:\Users\yostina\Desktop\project_data\data3.png")
