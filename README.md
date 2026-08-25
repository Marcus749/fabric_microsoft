# Microsoft Fabric 🚀

<div align="center">

### ☁️ End-to-End Data & Analytics Platform

**OneLake • Lakehouse • Data Factory • Pipelines • Dataflows Gen2 • Notebooks • Data Warehouse • SQL • Power BI**

<br>

![Microsoft Fabric](https://img.shields.io/badge/Microsoft%20Fabric-Analytics-0078D4?style=for-the-badge\&logo=microsoft)
![OneLake](https://img.shields.io/badge/OneLake-Data%20Lake-0078D4?style=for-the-badge\&logo=microsoft)
![Python](https://img.shields.io/badge/Python-Data%20Engineering-3776AB?style=for-the-badge\&logo=python)
![SQL](https://img.shields.io/badge/SQL-Analytics-CC2927?style=for-the-badge\&logo=microsoftsqlserver)
![Power BI](https://img.shields.io/badge/Power%20BI-Business%20Intelligence-F2C811?style=for-the-badge\&logo=powerbi)

</div>

---

## 📌 About This Repository

A comprehensive learning and hands-on repository covering **Microsoft Fabric**, Microsoft's end-to-end analytics and data platform.

This repository documents concepts, practical implementations, workflows, notebooks, pipelines, data engineering, data warehousing, OneLake, Lakehouse, and Power BI.

The goal of this repository is to demonstrate how modern data platforms can be used to:

```text
📥 INGEST
    ↓
💾 STORE
    ↓
🧹 CLEAN
    ↓
🔄 TRANSFORM
    ↓
⚙️ PROCESS
    ↓
🧮 ANALYZE
    ↓
📊 VISUALIZE
    ↓
💡 DELIVER INSIGHTS
```

---

# 📌 About Microsoft Fabric

**Microsoft Fabric** is an integrated, cloud-based analytics platform that brings together data engineering, data integration, data warehousing, data science, real-time analytics, and business intelligence in a unified environment.

Fabric provides a centralized ecosystem where data can move through the complete analytics lifecycle:

```text
                    ☁️ MICROSOFT FABRIC
                           │
                           ▼
                    📥 DATA SOURCES
                           │
                           ▼
                    🔄 DATA INGESTION
                           │
                           ▼
                     🌐 ONELAKE
                           │
                           ▼
                    🏞️ LAKEHOUSE
                           │
                           ▼
                 🧹 TRANSFORM & PROCESS
                           │
                 ┌─────────┴─────────┐
                 ▼                   ▼
          📓 NOTEBOOKS         🗄️ WAREHOUSE
                 │                   │
                 └─────────┬─────────┘
                           ▼
                    🧠 SEMANTIC MODEL
                           │
                           ▼
                      📊 POWER BI
                           │
                           ▼
                    💡 BUSINESS INSIGHTS
```

---

# 🏗️ Microsoft Fabric Architecture

The major components explored in this repository include:

```text
                         ☁️ MICROSOFT FABRIC
                                  │
             ┌────────────────────┼────────────────────┐
             │                    │                    │
             ▼                    ▼                    ▼
          🌐 ONELAKE          🏢 WORKSPACES       ⚡ CAPACITY
             │                    │                    │
             └────────────────────┼────────────────────┘
                                  │
       ┌──────────────────────────┼──────────────────────────┐
       │                          │                          │
       ▼                          ▼                          ▼
 🔧 DATA FACTORY             🏞️ LAKEHOUSE              🗄️ WAREHOUSE
       │                          │                          │
       ▼                          ▼                          ▼
 🔄 PIPELINES                 📓 NOTEBOOKS                 🧮 SQL
       │                          │                          │
       └──────────────────────────┼──────────────────────────┘
                                  │
                                  ▼
                           🧠 DATA ANALYTICS
                                  │
                                  ▼
                              📊 POWER BI
                                  │
                                  ▼
                           💡 INSIGHTS
```

---

# 📚 Topics Covered

This repository covers the following Microsoft Fabric concepts:

| #  | Topic                     | Area                  |
| -- | ------------------------- | --------------------- |
| 01 | 🚀 Microsoft Fabric       | Platform Overview     |
| 02 | 🏢 Workspaces             | Resource Management   |
| 03 | ⚡ Fabric Capacity         | Platform Capacity     |
| 04 | 🌐 OneLake                | Data Foundation       |
| 05 | 🏞️ Lakehouse             | Data Engineering      |
| 06 | 🔧 Data Factory           | Data Integration      |
| 07 | 🔄 Data Pipelines         | Orchestration         |
| 08 | 🔀 Dataflows Gen2         | Data Transformation   |
| 09 | 📓 Notebooks              | Data Processing       |
| 10 | ⚙️ Data Engineering       | Data Preparation      |
| 11 | 🗄️ Data Warehouse        | Data Warehousing      |
| 12 | 🧮 SQL Analytics          | Data Analysis         |
| 13 | 🧠 Semantic Models        | Data Modeling         |
| 14 | 📊 Power BI               | Business Intelligence |
| 15 | 🥇 Medallion Architecture | Data Architecture     |
| 16 | 🔁 End-to-End Workflows   | Analytics             |

---

# 🏢 Workspaces

A **Workspace** is a collaborative environment in Microsoft Fabric where users can create, organize, manage, and share Fabric items.

Typical workspace structure:

```text
🏢 Fabric Workspace
│
├── 🏞️ Lakehouse
│
├── 📓 Notebooks
│
├── 🔄 Pipelines
│
├── 🔀 Dataflows Gen2
│
├── 🗄️ Warehouse
│
├── 🧠 Semantic Model
│
├── 📊 Power BI Report
│
└── 📈 Dashboard
```

---

# 🌐 OneLake

**OneLake** is the unified data lake foundation of Microsoft Fabric.

It provides a centralized location for organizational data and helps create a common data foundation across Fabric workloads.

```text
                         🌐 ONELAKE
                            │
             ┌──────────────┼──────────────┐
             │              │              │
             ▼              ▼              ▼
        🏞️ Lakehouse    🗄️ Warehouse   📊 Analytics
             │              │              │
             └──────────────┼──────────────┘
                            ▼
                     Unified Data Layer
```

---

# 🏞️ Lakehouse

A **Lakehouse** combines capabilities of a data lake and a data warehouse.

It can work with:

* Structured data
* Semi-structured data
* Unstructured data
* Tables
* Files

### Lakehouse Structure

```text
🏞️ LAKEHOUSE
│
├── 📁 FILES
│   ├── 📄 CSV
│   ├── 📄 JSON
│   └── 📄 Other Files
│
└── 🗃️ TABLES
    ├── 👤 Customer
    ├── 💰 Sales
    ├── 📦 Product
    └── 🛒 Transactions
```

### Lakehouse Workflow

```text
📁 Raw Files
     ↓
🏞️ Lakehouse
     ↓
📓 Notebook
     ↓
🧹 Data Cleaning
     ↓
🔄 Transformation
     ↓
🗃️ Analytical Tables
```

---

# 🔄 Data Factory

Microsoft Fabric Data Factory provides capabilities for **data integration and orchestration**.

It can be used to:

* Connect to data sources
* Ingest data
* Transform data
* Schedule workflows
* Automate data movement
* Build data pipelines

### Data Factory Flow

```text
📁 CSV
  │
🗄️ Database
  │
🌐 API
  │
  └──────────────┐
                 ▼
          🔧 DATA FACTORY
                 │
                 ▼
            🔄 PIPELINE
                 │
                 ▼
             🌐 ONELAKE
                 │
                 ▼
            🏞️ LAKEHOUSE
```

---

# 🔗 Creating a Data Pipeline

A **Pipeline** is used to orchestrate and automate data workflows.

### Basic Pipeline

```text
┌──────────────────┐
│ 📁 DATA SOURCE   │
└────────┬─────────┘
         ↓
┌──────────────────┐
│ 🔄 COPY DATA     │
│    ACTIVITY      │
└────────┬─────────┘
         ↓
┌──────────────────┐
│ 🏞️ LAKEHOUSE     │
└────────┬─────────┘
         ↓
┌──────────────────┐
│ 📓 NOTEBOOK      │
│    ACTIVITY      │
└────────┬─────────┘
         ↓
┌──────────────────┐
│ 🧹 CLEAN &       │
│ 🔄 TRANSFORM     │
└────────┬─────────┘
         ↓
┌──────────────────┐
│ 🗃️ FINAL TABLE   │
└────────┬─────────┘
         ↓
┌──────────────────┐
│ 📊 POWER BI      │
└──────────────────┘
```

### Pipeline Features

* ⚙️ Activities
* 🔗 Dependencies
* 🎛️ Parameters
* 📦 Variables
* ⏰ Scheduling
* 📊 Monitoring
* 🚨 Error Handling
* 🔄 Automated Execution

---

# 📓 Fabric Notebooks

Microsoft Fabric Notebooks provide an interactive environment for data engineering, data analysis, and data transformation.

Python and Spark can be used to process and analyze datasets.

### Notebook Workflow

```text
📥 LOAD DATA
     ↓
🔍 EXPLORE DATA
     ↓
🧹 CLEAN DATA
     ↓
🔄 TRANSFORM DATA
     ↓
📊 ANALYZE DATA
     ↓
💾 SAVE RESULTS
```

### Example Notebook

```python
# Read data
df = spark.read.csv(
    "Files/data.csv",
    header=True,
    inferSchema=True
)

# Display data
display(df)

# Remove duplicate records
df = df.dropDuplicates()

# Save processed data
df.write.mode("overwrite").format("delta").saveAsTable(
    "processed_data"
)
```

---

# 🧹 Data Cleaning & Transformation

Data cleaning is an important part of the data engineering workflow.

Common operations include:

* Removing duplicates
* Handling missing values
* Correcting data types
* Renaming columns
* Filtering records
* Standardizing values
* Creating calculated columns
* Joining datasets
* Aggregating data

### Data Cleaning Flow

```text
              📥 RAW DATA
                   │
                   ▼
            🔍 DATA PROFILING
                   │
                   ▼
            🧹 MISSING VALUES
                   │
                   ▼
            🗑️ DUPLICATES
                   │
                   ▼
             🔤 DATA TYPES
                   │
                   ▼
            🔄 TRANSFORMATION
                   │
                   ▼
              ✅ CLEAN DATA
```

---

# 🔀 Dataflows Gen2

**Dataflows Gen2** provides a low-code approach to data ingestion and transformation.

### Workflow

```text
📥 DATA SOURCE
      ↓
🔀 DATAFLOW GEN2
      ↓
🧹 TRANSFORM
      ↓
🔍 VALIDATE
      ↓
📤 DESTINATION
      ↓
🏞️ LAKEHOUSE / 🗄️ WAREHOUSE
```

It can be useful when transformations need to be performed without writing extensive code.

---

# 🏗️ Medallion Architecture

The repository also explores the **Medallion Architecture**, a common approach for organizing data processing layers.

```text
                         📥 RAW DATA
                              │
                              ▼
                    ┌─────────────────┐
                    │ 🥉 BRONZE       │
                    │ Raw Data        │
                    └────────┬────────┘
                             ↓
                    ┌─────────────────┐
                    │ 🥈 SILVER       │
                    │ Cleaned Data    │
                    └────────┬────────┘
                             ↓
                    ┌─────────────────┐
                    │ 🥇 GOLD         │
                    │ Business Data   │
                    └────────┬────────┘
                             ↓
                    ┌─────────────────┐
                    │ 📊 POWER BI     │
                    └────────┬────────┘
                             ↓
                       💡 INSIGHTS
```

### 🥉 Bronze

Contains raw or minimally processed data.

### 🥈 Silver

Contains cleaned and transformed data.

### 🥇 Gold

Contains business-ready and analytics-ready data.

---

# 🗄️ Data Warehouse

Microsoft Fabric provides a dedicated **Data Warehouse** experience for structured analytical workloads.

It allows users to work with:

* Tables
* Views
* SQL
* Relationships
* Analytical queries
* Data models

### Warehouse Workflow

```text
🏞️ SOURCE DATA
      ↓
🗄️ DATA WAREHOUSE
      ↓
🧮 SQL QUERIES
      ↓
📊 ANALYSIS
      ↓
🧠 SEMANTIC MODEL
      ↓
📈 POWER BI
```

### Example SQL

```sql
SELECT
    Product,
    SUM(Sales) AS Total_Sales
FROM Sales
GROUP BY Product
ORDER BY Total_Sales DESC;
```

---

# 🧮 SQL Analytics

SQL can be used to analyze data stored in Fabric.

```sql
SELECT
    Customer_ID,
    COUNT(*) AS Total_Orders,
    SUM(Amount) AS Total_Spending
FROM Orders
GROUP BY Customer_ID
ORDER BY Total_Spending DESC;
```

This can help generate business insights such as:

* 👑 Top customers
* 🏆 Best-selling products
* 💰 Total revenue
* 📈 Order trends
* 👤 Customer behavior

---

# 🧠 Semantic Model

A semantic model provides a business-oriented layer for analytical data.

```text
🏞️ LAKEHOUSE
      │
      ├──────────────┐
      │              │
      ▼              ▼
🗄️ WAREHOUSE     📊 DATA
      │              │
      └──────┬───────┘
             ↓
      🧠 SEMANTIC MODEL
             │
      ┌──────┼──────┐
      ▼      ▼      ▼
    Sales  Customer Product
      │      │      │
      └──────┼──────┘
             ↓
         📊 POWER BI
```

---

# 📊 Power BI

Power BI is used to transform processed data into interactive reports and dashboards.

### Power BI Workflow

```text
📥 DATA SOURCE
      ↓
🌐 ONELAKE
      ↓
🏞️ LAKEHOUSE / 🗄️ WAREHOUSE
      ↓
🧠 SEMANTIC MODEL
      ↓
📊 POWER BI
      ↓
📈 REPORT / DASHBOARD
      ↓
💡 BUSINESS INSIGHTS
```

Power BI can be used for:

* 📊 Interactive dashboards
* 📈 Data visualization
* 🎯 KPI tracking
* 💼 Business intelligence
* 📉 Trend analysis
* 💡 Decision making

---

# 📈 Data Visualization

Common visualizations explored include:

* 📊 Bar Charts
* 📈 Line Charts
* 🥧 Pie / Donut Charts
* 📋 Tables
* 🎯 Cards
* 📌 KPI Indicators
* 🗺️ Maps
* 🎚️ Slicers
* 🔍 Interactive Filters

### Example Dashboard

```text
┌──────────────────────────────────────────────┐
│             📊 BUSINESS DASHBOARD            │
├────────────┬────────────┬─────────┬─────────┤
│ 💰 Revenue │ 🛒 Orders  │ 👤 Users │ 📈 Growth│
├────────────┴────────────┴─────────┴─────────┤
│                                              │
│              📈 SALES TREND                 │
│                                              │
├────────────────────────┬─────────────────────┤
│ 📦 PRODUCT PERFORMANCE  │ 👤 CUSTOMER ANALYSIS│
│                        │                     │
├────────────────────────┴─────────────────────┤
│              🎚️ FILTERS / SLICERS           │
└──────────────────────────────────────────────┘
```

---

# 🔁 End-to-End Microsoft Fabric Project

One of the main objectives of this repository is to understand how different Fabric components work together.

### Complete Workflow

```text
                     🌐 DATA SOURCES
                            │
              ┌─────────────┼─────────────┐
              │             │             │
             📁 CSV       🗄️ SQL        🌐 API
              │             │             │
              └─────────────┼─────────────┘
                            ▼
                     🔧 DATA FACTORY
                            │
                            ▼
                       🔄 PIPELINE
                            │
                            ▼
                         🌐 ONELAKE
                            │
                            ▼
                       🏞️ LAKEHOUSE
                            │
                            ▼
                        📓 NOTEBOOK
                            │
                  ┌─────────┴─────────┐
                  ▼                   ▼
              🧹 CLEANING       🔄 TRANSFORMATION
                  │                   │
                  └─────────┬─────────┘
                            ▼
                       🗃️ DELTA TABLE
                            │
                            ▼
                      🗄️ DATA WAREHOUSE
                            │
                            ▼
                      🧠 SEMANTIC MODEL
                            │
                            ▼
                         📊 POWER BI
                            │
                            ▼
                    💡 BUSINESS INSIGHTS
```

---

# 🧪 Hands-On Activities

This repository contains practical exploration of Microsoft Fabric, including:

### 1. 🏢 Workspace Creation

* Creating a Fabric workspace
* Understanding workspace structure
* Managing Fabric items

### 2. 🏞️ Lakehouse

* Creating a Lakehouse
* Uploading files
* Creating tables
* Exploring Files and Tables sections

### 3. 🔄 Data Pipeline

* Creating a pipeline
* Adding activities
* Connecting data sources
* Copying data
* Creating dependencies
* Running pipelines
* Monitoring execution

### 4. 📓 Notebook

* Creating notebooks
* Reading datasets
* Using PySpark
* Data cleaning
* Data transformation
* Creating tables
* Saving processed data

### 5. 🔀 Dataflow Gen2

* Creating dataflows
* Connecting sources
* Transforming data
* Loading data into Fabric destinations

### 6. 🗄️ Data Warehouse

* Creating warehouse objects
* Creating tables
* Running SQL queries
* Performing analytical operations

### 7. 📊 Power BI

* Connecting to Fabric data
* Creating semantic models
* Building visualizations
* Designing interactive reports
* Creating dashboards

---

# 📂 Repository Structure

```text
fabric_microsoft/
│
├── 📄 README.md
│
├── 🏗️ architecture/
│   ├── fabric_architecture.md
│   ├── onelake.md
│   └── medallion_architecture.md
│
├── 🏢 workspaces/
│   └── workspace_notes.md
│
├── 🌐 onelake/
│   └── onelake_notes.md
│
├── 🏞️ lakehouse/
│   ├── lakehouse_notes.md
│   └── datasets/
│
├── 🔄 pipelines/
│   ├── pipeline_notes.md
│   └── pipeline_workflows/
│
├── 📓 notebooks/
│   ├── data_cleaning.ipynb
│   ├── data_transformation.ipynb
│   └── data_analysis.ipynb
│
├── 🔀 dataflows/
│   └── dataflow_notes.md
│
├── 🗄️ warehouse/
│   ├── sql_queries.sql
│   └── warehouse_notes.md
│
├── 🧠 semantic_models/
│   └── model_notes.md
│
├── 📊 powerbi/
│   ├── dashboards/
│   └── reports/
│
├── 📁 datasets/
│   ├── raw/
│   └── processed/
│
└── 📸 screenshots/
    ├── workspace/
    ├── onelake/
    ├── lakehouse/
    ├── pipelines/
    ├── notebooks/
    ├── warehouse/
    └── powerbi/
```

---

# 🎯 Learning Objectives

Through this repository, I aim to develop practical knowledge of:

```text
☁️ Modern Data Platforms
        ↓
🔧 Data Engineering
        ↓
📥 Data Ingestion
        ↓
🔄 ETL / ELT
        ↓
🧹 Data Cleaning
        ↓
⚙️ Data Transformation
        ↓
🌐 Data Lake Architecture
        ↓
🏞️ Lakehouse Architecture
        ↓
🗄️ Data Warehousing
        ↓
🐍 PySpark
        ↓
🧮 SQL Analytics
        ↓
📊 Business Intelligence
        ↓
📈 Data Visualization
        ↓
💡 Business Insights
```

---

# 💡 Key Concepts

| Concept              | Purpose                                       |
| -------------------- | --------------------------------------------- |
| **Microsoft Fabric** | Unified analytics platform                    |
| **Workspace**        | Organizes Fabric resources                    |
| **OneLake**          | Unified organizational data lake              |
| **Lakehouse**        | Combines data lake and warehouse capabilities |
| **Data Factory**     | Data integration and orchestration            |
| **Pipeline**         | Automates data workflows                      |
| **Dataflow Gen2**    | Low-code data transformation                  |
| **Notebook**         | Code-based data processing and analysis       |
| **Warehouse**        | Structured analytical data storage            |
| **SQL**              | Data querying and analysis                    |
| **Semantic Model**   | Defines analytical data relationships         |
| **Power BI**         | Visualization and business intelligence       |

---

# 🔐 Data & Governance

Modern analytics platforms require proper data management.

Important areas include:

* 🔐 Data security
* 👥 Access management
* 🏛️ Data governance
* ✅ Data quality
* 🔗 Data lineage
* 📊 Data monitoring
* 🏢 Workspace management
* 🛡️ Controlled data access

These concepts are important for building reliable, secure, and scalable analytics solutions.

---

# 🗺️ Microsoft Fabric Learning Roadmap

```text
                         🚀 MICROSOFT FABRIC
                                  │
                                  ▼
                           🏢 WORKSPACES
                                  │
                                  ▼
                              🌐 ONELAKE
                                  │
                                  ▼
                           🏞️ LAKEHOUSE
                                  │
                                  ▼
                         🔧 DATA FACTORY
                                  │
                                  ▼
                            🔄 PIPELINES
                                  │
                                  ▼
                            📓 NOTEBOOKS
                                  │
                                  ▼
                        ⚙️ DATA ENGINEERING
                                  │
                                  ▼
                         🗄️ DATA WAREHOUSE
                                  │
                                  ▼
                              🧮 SQL
                                  │
                                  ▼
                         🧠 SEMANTIC MODEL
                                  │
                                  ▼
                            📊 POWER BI
                                  │
                                  ▼
                           💡 INSIGHTS
```

---

# 🚀 Future Additions

Planned additions to this repository include:

* 🔄 Advanced Data Factory pipelines
* 🎛️ Parameterized pipelines
* 📊 Pipeline monitoring
* 🐍 Advanced PySpark transformations
* 📥 Incremental data loading
* 🥇 Medallion Architecture implementation
* 🗄️ Data Warehouse projects
* 🧮 Advanced SQL analytics
* 📊 Power BI dashboards
* ⚡ Real-time analytics
* 🤖 Data science workflows
* 🔁 End-to-end business intelligence projects
* 📚 Microsoft Fabric best practices

---

# 🏆 Skills Demonstrated

<div align="center">

**Microsoft Fabric** • **OneLake** • **Lakehouse** • **Data Factory** • **Pipelines** • **Dataflows Gen2** • **Notebooks** • **PySpark** • **SQL** • **Data Engineering** • **Data Warehousing** • **Semantic Modeling** • **Power BI** • **Data Visualization** • **ETL/ELT** • **Data Analytics**

</div>

---

# 📌 Repository Purpose

This repository serves as a **learning portfolio and practical reference for Microsoft Fabric**.

It documents my journey from understanding Fabric fundamentals to building complete data workflows involving:

```text
📥 INGEST
   ↓
🌐 STORE
   ↓
🧹 CLEAN
   ↓
🔄 TRANSFORM
   ↓
⚙️ PROCESS
   ↓
🗄️ ANALYZE
   ↓
📊 VISUALIZE
   ↓
💡 INSIGHTS
```

> **Learn → Build → Analyze → Visualize → Improve**

---

# ⭐ If You Find This Repository Useful

If this repository helps you understand **Microsoft Fabric, Data Engineering, Data Analytics, or Business Intelligence**, consider giving it a ⭐ **Star** and exploring the projects and examples available in the repository.

---

# 👨‍💻 Author

<div align="center">

## **Gyan Prakash Patel**

**B.Tech (Hons.) – Computer Science & Engineering**
**Specialization: Data Science & Artificial Intelligence**

### 💻 Data Analytics | 🔧 Data Engineering | ☁️ Microsoft Fabric | 🧮 SQL | 🐍 Python | 📊 Power BI | 🤖 AI

</div>

---

# 📜 Disclaimer

This repository is created for **educational, learning, and portfolio purposes**.

The examples and implementations are intended to demonstrate concepts and practical workflows using **Microsoft Fabric**.

---

<div align="center">

### ☁️ Microsoft Fabric

**From Data → to Insights**

**📥 Ingest → 💾 Store → 🔄 Transform → 🧮 Analyze → 📊 Visualize → 💡 Decide**

⭐ **Keep Learning • Keep Building • Keep Analyzing** ⭐

</div>
