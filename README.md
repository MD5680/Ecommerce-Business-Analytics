# Ecommerce Business Analytics

A complete **E-commerce Data Engineering and Analytics project** built using **Databricks**. The project demonstrates an end-to-end data pipeline, including data ingestion, data quality, data exploration, data modeling, dimensional/fact tables, and business analysis.

The project uses **Databricks notebooks and a Databricks Job/Asset Bundle** to organize and automate the main data processing workflow.

---

## Project Overview

The objective of this project is to process e-commerce data through multiple stages and transform raw data into structured datasets that can be used for business analysis.

The project follows a data engineering workflow:

```text
Raw Data
   ↓
Data Ingestion
   ↓
Data Quality
   ↓
Data Exploration
   ↓
Data Cleaning / Modeling
   ↓
Fact & Dimension Tables
   ↓
Gold Business Tables
   ↓
Business Analysis
```

---

## Project Objectives

* Ingest e-commerce data into Databricks
* Perform data quality checks
* Explore and understand the dataset
* Clean and transform data
* Build fact and dimension tables
* Create business-ready tables
* Perform SQL-based business analysis
* Automate the main workflow using a Databricks Job
* Manage notebooks and job configuration using GitHub

---

## Project Structure

```text
Ecommerce-Business-Analytics/
│
├── data_ingestion.ipynb
├── Data_Quality.ipynb
├── Data_Exploration.ipynb
├── Data_Cleaning.ipynb
├── Data_Modeling.ipynb
├── dimensions.ipynb
├── fact_sales.ipynb
├── gold_business_tables.ipynb
├── Advanced_sql_analysis.ipynb
│
├── ecommerce-pipeline/
│   ├── databricks.yml
│   ├── README.md
│   │
│   └── resources/
│       └── ecommerce_data_engineering_pipeline.job.yml
│
└── .gitignore
```

---

## Databricks Pipeline / Job

The main Databricks Job contains **3 tasks**:

```text
data_ingestion
      ↓
Data_Quality
      ↓
Data_Exploration
```

### 1. Data Ingestion

The `data_ingestion` notebook is the starting point of the workflow.

It is responsible for bringing the required e-commerce data into the Databricks environment for further processing.

### 2. Data Quality

The `Data_Quality` notebook runs after data ingestion.

It is used to perform data quality-related checks before the data is used for further analysis.

### 3. Data Exploration

The `Data_Exploration` notebook runs after the data quality task.

It is used to explore the processed data and understand patterns and information available in the dataset.

---

## Notebooks

### `data_ingestion`

Handles the initial data ingestion process.

### `Data_Quality`

Performs data quality checks on the ingested data.

### `Data_Exploration`

Explores the available data using Databricks/Spark/SQL.

### `Data_Cleaning`

Used for cleaning and preparing data for further processing.

### `Data_Modeling`

Handles data transformation and modeling.

### `dimensions`

Creates or prepares dimension-related tables used in the analytical model.

### `fact_sales`

Creates or prepares the sales fact table.

### `gold_business_tables`

Creates business-ready tables for analytical use.

### `Advanced_sql_analysis`

Performs advanced SQL-based analysis on the processed data.

---

## Data Modeling

The project includes a dimensional modeling approach with:

* Fact tables
* Dimension tables
* Business-ready analytical tables

The main analytical fact table is:

```text
fact_sales
```

Dimension-related processing is handled through:

```text
dimensions
```

Business-level outputs are handled through:

```text
gold_business_tables
```

---

## Technologies Used

| Technology                   | Purpose                                   |
| ---------------------------- | ----------------------------------------- |
| **Databricks**               | Data engineering and analytics platform   |
| **Apache Spark / PySpark**   | Data processing                           |
| **SQL**                      | Data querying and analysis                |
| **Python**                   | Data processing and notebook development  |
| **Delta/Databricks Tables**  | Data storage and analytical processing    |
| **Git**                      | Version control                           |
| **GitHub**                   | Source-code and project management        |
| **Databricks Asset Bundles** | Job/resource deployment and configuration |

---

## Databricks Asset Bundle

The Databricks Job configuration is maintained as YAML inside the project.

```text
ecommerce-pipeline/
│
├── databricks.yml
│
└── resources/
    └── ecommerce_data_engineering_pipeline.job.yml
```

The job YAML defines the Databricks Job and its task dependencies.

Example workflow:

```text
data_ingestion
      │
      ▼
Data_Quality
      │
      ▼
Data_Exploration
```

This allows the job configuration to be maintained as code and version-controlled through GitHub.

---

## GitHub Integration

The project is maintained in Git using a Databricks Git folder.

The repository contains:

* Databricks notebooks
* Databricks Asset Bundle configuration
* Job YAML
* Project documentation
* Git configuration files

This provides version control and makes the project easier to maintain and reproduce.

---

## How to Run the Project

### Step 1 — Open Databricks

Open the Databricks workspace and access the project notebooks.

### Step 2 — Run Data Ingestion

Run:

```text
data_ingestion
```

### Step 3 — Run Data Quality

Run:

```text
Data_Quality
```

after successful data ingestion.

### Step 4 — Run Data Exploration

Run:

```text
Data_Exploration
```

after the data quality task completes successfully.

### Step 5 — Continue Data Processing

The remaining notebooks can then be used for:

```text
Data Cleaning
      ↓
Data Modeling
      ↓
Dimensions / Fact Tables
      ↓
Gold Business Tables
      ↓
Advanced SQL Analysis
```

### Step 6 — Run the Databricks Job

The main automated Job can execute the three configured tasks:

```text
data_ingestion → Data_Quality → Data_Exploration
```

---

## Business Analysis

After the data has been processed and modeled, the project can be used to perform business analysis such as:

* Sales analysis
* Product analysis
* Customer-related analysis
* Business performance analysis
* Aggregated sales analysis
* SQL-based analytical queries

The `Advanced_sql_analysis` notebook contains advanced SQL analysis performed on the processed data.

---

## Repository Contents

```text
 Ecommerce-Business-Analytics
│
├──  Data Engineering Notebooks
│   ├── data_ingestion
│   ├── Data_Quality
│   ├── Data_Exploration
│   ├── Data_Cleaning
│   ├── Data_Modeling
│   ├── dimensions
│   ├── fact_sales
│   ├── gold_business_tables
│   └── Advanced_sql_analysis
│
├──  Databricks Pipeline
│   └── ecommerce-pipeline
│       ├── databricks.yml
│       └── resources/
│           └── ecommerce_data_engineering_pipeline.job.yml
│
├──  README.md
│
└──  .gitignore
```

---

## Key Learning Outcomes

Through this project, the following concepts are demonstrated:

* Data ingestion
* Data quality validation
* Data exploration
* Data cleaning
* Data transformation
* Data modeling
* Fact and dimension tables
* Business-ready data
* SQL analytics
* Databricks Jobs
* Databricks Asset Bundles
* Git and GitHub integration
* Version control
* Workflow orchestration

---

## Author

**Mohammed Azam**

B.Sc. Computer Science
Central University of Karnataka

### Skills Demonstrated

```text
Python
SQL
PySpark
Databricks
Apache Spark
Data Engineering
Data Modeling
Git
GitHub
Data Analytics
```

---

## Project Status

**Completed**

The project includes the Databricks notebooks, data processing workflow, analytical components, and Databricks Job configuration maintained through GitHub.
