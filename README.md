# Microsoft Fabric 🚀

A comprehensive learning and hands-on repository covering **Microsoft Fabric**, Microsoft's end-to-end analytics and data platform. This repository documents concepts, practical implementations, workflows, notebooks, pipelines, data engineering, data warehousing, OneLake, Lakehouse, and Power BI.

The goal of this repository is to demonstrate how modern data platforms can be used to **ingest, transform, process, analyze, visualize, and deliver data-driven insights** using Microsoft Fabric.

---

## 📌 About Microsoft Fabric

**Microsoft Fabric** is an integrated, cloud-based analytics platform that brings together data engineering, data integration, data warehousing, data science, real-time analytics, and business intelligence in a unified environment.

Fabric provides a centralized ecosystem where data can move through the complete analytics lifecycle:

```text
Data Sources
     ↓
Data Ingestion
     ↓
Data Storage
     ↓
Data Transformation
     ↓
Data Engineering / Data Warehouse
     ↓
Data Analysis
     ↓
Power BI
     ↓
Business Insights
```

A major component of Fabric is **OneLake**, which acts as a unified data lake for the organization.

---

# 🏗️ Microsoft Fabric Architecture

The major components explored in this repository include:

```text
                         Microsoft Fabric
                                │
             ┌──────────────────┼──────────────────┐
             │                  │                  │
          OneLake            Workspaces         Capacity
             │                  │                  │
             └──────────────────┼──────────────────┘
                                │
        ┌───────────────────────┼────────────────────────┐
        │                       │                        │
   Data Engineering       Data Integration        Data Warehouse
        │                       │                        │
     Lakehouse              Data Factory           Warehouse
     Notebooks               Pipelines              SQL
        │                       │
        └───────────────────────┼───────────────────────┘
                                │
                         Data Analytics
                                │
                            Power BI
```

---

# 📚 Topics Covered

This repository covers the following Microsoft Fabric concepts:

* Microsoft Fabric Overview
* Fabric Architecture
* Workspaces
* Fabric Capacity
* Domains
* OneLake
* Lakehouse
* Data Factory
* Data Pipelines
* Dataflows Gen2
* Notebooks
* Data Engineering
* Data Warehouse
* SQL Analytics
* Power BI
* Data Ingestion
* Data Transformation
* Data Cleaning
* ETL / ELT
* Medallion Architecture
* Data Modeling
* Data Visualization
* End-to-End Data Workflows

---

# 🏢 Workspaces

A **Workspace** is a collaborative environment in Microsoft Fabric where users can create, organize, manage, and share Fabric items.

Typical workspace items include:

* Lakehouses
* Warehouses
* Notebooks
* Pipelines
* Dataflows
* Semantic Models
* Power BI Reports
* Dashboards

Example workspace structure:

```text
Fabric Workspace
│
├── 📁 Lakehouse
├── 📓 Notebooks
├── 🔄 Pipelines
├── 🔀 Dataflows
├── 🗄️ Warehouse
├── 📊 Semantic Model
└── 📈 Power BI Report
```

---

# 🌐 OneLake

**OneLake** is the unified data lake foundation of Microsoft Fabric.

It provides a centralized location for organizational data and helps eliminate unnecessary data duplication across different analytics workloads.

```text
                    OneLake
                       │
        ┌──────────────┼──────────────┐
        │              │              │
     Lakehouse      Warehouse      Other Data
        │
   ┌────┴────┐
   │         │
Tables    Files
```

OneLake can support different Fabric workloads while maintaining a unified data foundation.

---

# 🏞️ Lakehouse

A **Lakehouse** combines capabilities of a data lake and a data warehouse.

It can store:

* Structured data
* Semi-structured data
* Unstructured data
* Tables
* Files

A typical Lakehouse contains:

```text
Lakehouse
│
├── Files
│   ├── CSV
│   ├── JSON
│   └── Other Files
│
└── Tables
    ├── Customer
    ├── Sales
    ├── Product
    └── Transactions
```

Lakehouses are particularly useful for data engineering and analytics workloads.

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

Example:

```text
CSV / Database / API
        ↓
   Data Factory
        ↓
    Pipeline
        ↓
    Lakehouse
        ↓
 Transformation
        ↓
   Power BI
```

---

# 🔗 Creating a Data Pipeline

A **Pipeline** is used to orchestrate and automate data workflows.

A basic pipeline can be designed as:

```text
Source
  ↓
Copy Data
  ↓
Lakehouse
  ↓
Data Transformation
  ↓
Notebook
  ↓
Final Table
```

### Example Pipeline Workflow

```text
CSV File
   │
   ▼
Copy Data Activity
   │
   ▼
Lakehouse Files
   │
   ▼
Notebook Activity
   │
   ▼
Clean & Transform Data
   │
   ▼
Lakehouse Table
   │
   ▼
Power BI
```

Pipelines can also be configured with:

* Activities
* Parameters
* Variables
* Scheduling
* Dependencies
* Monitoring
* Error handling

---

# 📓 Fabric Notebooks

Microsoft Fabric Notebooks provide an interactive environment for data engineering, data analysis, and data transformation.

Python and Spark can be used to process large datasets.

Typical notebook workflow:

```text
Load Data
    ↓
Inspect Data
    ↓
Clean Data
    ↓
Transform Data
    ↓
Analyze Data
    ↓
Save Results
```

### Example Notebook Operations

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

Example:

```text
Raw Data
   ↓
Missing Value Handling
   ↓
Duplicate Removal
   ↓
Data Type Correction
   ↓
Transformation
   ↓
Clean Data
```

---

# 🔀 Dataflows Gen2

**Dataflows Gen2** provides a low-code approach to data ingestion and transformation.

A typical workflow:

```text
Data Source
     ↓
Dataflow Gen2
     ↓
Transform Data
     ↓
Destination
     ↓
Lakehouse / Warehouse
```

It can be useful when transformations need to be performed without writing extensive code.

---

# 🏗️ Medallion Architecture

The repository also explores the **Medallion Architecture**, a common approach for organizing data processing layers.

```text
              Raw Data
                 │
                 ▼
          🥉 Bronze Layer
                 │
                 ▼
           🥈 Silver Layer
                 │
                 ▼
             🥇 Gold Layer
                 │
                 ▼
             Power BI
```

### 🥉 Bronze

Contains raw or minimally processed data.

### 🥈 Silver

Contains cleaned and transformed data.

### 🥇 Gold

Contains business-ready and analytics-ready data.

Example:

```text
Bronze
  ↓
Raw Sales Data

Silver
  ↓
Clean Sales Data

Gold
  ↓
Sales Summary
Customer Insights
Product Performance
```

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

Example:

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

Example:

```sql
SELECT
    Customer_ID,
    COUNT(*) AS Total_Orders,
    SUM(Amount) AS Total_Spending
FROM Orders
GROUP BY Customer_ID;
```

This can help generate business insights such as:

* Top customers
* Best-selling products
* Total revenue
* Order trends
* Customer behavior

---

# 📊 Power BI

Power BI is used to transform processed data into interactive reports and dashboards.

Typical workflow:

```text
Data Source
    ↓
OneLake
    ↓
Lakehouse / Warehouse
    ↓
Semantic Model
    ↓
Power BI
    ↓
Dashboard / Report
```

Power BI can be used for:

* Interactive dashboards
* Data visualization
* KPI tracking
* Business intelligence
* Trend analysis
* Decision making

---

# 📈 Data Visualization

Common visualizations explored include:

* Bar Charts
* Line Charts
* Pie / Donut Charts
* Tables
* Cards
* KPI Indicators
* Maps
* Slicers
* Interactive Filters

Example dashboard structure:

```text
┌──────────────────────────────────────────┐
│             BUSINESS DASHBOARD           │
├──────────┬──────────┬──────────┬─────────┤
│ Revenue  │ Orders   │ Customers│ Growth  │
├──────────┴──────────┴──────────┴─────────┤
│                                          │
│          Sales Trend                    │
│                                          │
├────────────────────┬─────────────────────┤
│ Product Performance│ Customer Analysis   │
│                    │                     │
└────────────────────┴─────────────────────┘
```

---

# 🔁 End-to-End Microsoft Fabric Project

One of the main objectives of this repository is to understand how different Fabric components work together.

### Complete Workflow

```text
              DATA SOURCES
                   │
        ┌──────────┼──────────┐
        │          │          │
       CSV       SQL DB      API
        │          │          │
        └──────────┼──────────┘
                   ▼
             DATA FACTORY
                   │
                   ▼
               PIPELINE
                   │
                   ▼
                ONELAKE
                   │
                   ▼
              LAKEHOUSE
                   │
                   ▼
              NOTEBOOK
                   │
          ┌────────┴────────┐
          ▼                 ▼
       CLEANING         TRANSFORMATION
          │                 │
          └────────┬────────┘
                   ▼
             DELTA TABLE
                   │
                   ▼
              DATA WAREHOUSE
                   │
                   ▼
             SEMANTIC MODEL
                   │
                   ▼
                POWER BI
                   │
                   ▼
          BUSINESS INSIGHTS
```

---

# 🧪 Hands-On Activities

This repository contains practical exploration of Microsoft Fabric, including:

### 1. Workspace Creation

* Creating a Fabric workspace
* Understanding workspace structure
* Managing Fabric items

### 2. Lakehouse

* Creating a Lakehouse
* Uploading files
* Creating tables
* Exploring Files and Tables sections

### 3. Data Pipeline

* Creating a pipeline
* Adding activities
* Connecting data sources
* Copying data
* Creating dependencies
* Running pipelines
* Monitoring execution

### 4. Notebook

* Creating notebooks
* Reading datasets
* Using PySpark
* Data cleaning
* Data transformation
* Creating tables
* Saving processed data

### 5. Dataflow Gen2

* Creating dataflows
* Connecting sources
* Transforming data
* Loading data into Fabric destinations

### 6. Data Warehouse

* Creating warehouse objects
* Creating tables
* Running SQL queries
* Performing analytical operations

### 7. Power BI

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
├── README.md
│
├── architecture/
│   ├── fabric_architecture.md
│   ├── onelake.md
│   └── medallion_architecture.md
│
├── workspaces/
│   └── workspace_notes.md
│
├── lakehouse/
│   ├── lakehouse_notes.md
│   └── datasets/
│
├── pipelines/
│   ├── pipeline_notes.md
│   └── pipeline_workflows/
│
├── notebooks/
│   ├── data_cleaning.ipynb
│   ├── data_transformation.ipynb
│   └── data_analysis.ipynb
│
├── dataflows/
│   └── dataflow_notes.md
│
├── warehouse/
│   ├── sql_queries.sql
│   └── warehouse_notes.md
│
├── powerbi/
│   ├── dashboards/
│   └── reports/
│
├── datasets/
│   ├── raw/
│   └── processed/
│
└── screenshots/
    ├── workspace/
    ├── lakehouse/
    ├── pipelines/
    ├── notebooks/
    └── powerbi/
```

---

# 🎯 Learning Objectives

Through this repository, I aim to develop practical knowledge of:

* Modern data platforms
* Cloud data engineering
* Data ingestion
* ETL / ELT pipelines
* Data transformation
* Data lake architecture
* Data warehousing
* Distributed data processing
* PySpark
* SQL analytics
* Business intelligence
* Data visualization
* End-to-end analytics workflows

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

* Data security
* Access management
* Data governance
* Data quality
* Data lineage
* Data monitoring
* Workspace management
* Controlled data access

These concepts are important for building reliable and scalable analytics solutions.

---

# 🚀 Future Additions

Planned additions to this repository include:

* Advanced Data Factory pipelines
* Parameterized pipelines
* Pipeline monitoring
* Advanced PySpark transformations
* Incremental data loading
* Medallion Architecture implementation
* Data Warehouse projects
* Advanced SQL analytics
* Power BI dashboards
* Real-time analytics
* Data science workflows
* End-to-end business intelligence projects
* Microsoft Fabric best practices

---

# 🏆 Skills Demonstrated

This repository demonstrates practical exposure to:

**Microsoft Fabric • OneLake • Lakehouse • Data Factory • Pipelines • Dataflows Gen2 • Notebooks • PySpark • SQL • Data Engineering • Data Warehousing • Power BI • Data Visualization • ETL/ELT • Data Analytics**

---

# 📌 Repository Purpose

This repository serves as a **learning portfolio and practical reference for Microsoft Fabric**. It documents my journey from understanding Fabric fundamentals to building complete data workflows involving ingestion, transformation, storage, analysis, and visualization.

> **Learn → Build → Analyze → Visualize → Improve**

---

## ⭐ If You Find This Repository Useful

If this repository helps you understand Microsoft Fabric or its components, consider giving it a ⭐ **Star** and exploring the projects and examples available in the repository.

---

## 👨‍💻 Author

**Gyan Prakash Patel**

B.Tech (Hons.) – Computer Science & Engineering
**Specialization:** Data Science & Artificial Intelligence

Interested in:

**Data Analytics | Data Engineering | Microsoft Fabric | SQL | Python | Power BI | Artificial Intelligence**

---

## 📜 Disclaimer

This repository is created for **educational, learning, and portfolio purposes**. The examples and implementations are intended to demonstrate concepts and practical workflows using Microsoft Fabric.
