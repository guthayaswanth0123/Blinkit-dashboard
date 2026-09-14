# 🛒 Blinkit Business Intelligence Dashboard

### End-to-End Retail Analytics & Business Intelligence System

> A student-built Business Intelligence project that integrates **MySQL, Python ETL, and Microsoft Power BI** to analyze sales, customers, inventory, marketing campaigns, and customer feedback for a simulated Quick-Commerce business environment.

---

## 📌 Project Overview

The **Blinkit Business Intelligence Dashboard** is an end-to-end data analytics project developed to demonstrate how raw transactional and operational data can be transformed into meaningful business insights.

The project simulates a real-world **Quick-Commerce Analytics System**, where business teams need to monitor:

* Sales and revenue performance
* Customer acquisition and retention
* Product performance
* Inventory availability
* Marketing campaign effectiveness
* Customer satisfaction
* Operational performance

The complete data pipeline starts with raw CSV/Excel data, processes and cleans the data using **Python**, stores structured data in **MySQL**, performs analytical transformations using **SQL**, and finally presents business insights through an interactive **Power BI dashboard**.

---

# 🎯 Project Objectives

The main objectives of this project are:

1. Transform raw retail data into structured and analysis-ready datasets.
2. Build a normalized relational database using MySQL.
3. Automate data cleaning and transformation using Python.
4. Perform multi-table SQL analysis using joins, aggregations, subqueries, and indexing.
5. Develop an interactive Power BI dashboard for business decision-making.
6. Analyze customer purchasing behavior and retention.
7. Monitor inventory availability and identify potential stock issues.
8. Evaluate marketing campaign performance and ROI.
9. Analyze customer feedback and ratings.
10. Demonstrate an end-to-end **ETL → Database → BI** workflow.

---

# 🧰 Technology Stack

| Category              | Technology             |
| --------------------- | ---------------------- |
| Database              | MySQL                  |
| Database Tool         | MySQL Workbench        |
| Programming           | Python                 |
| Data Processing       | Pandas, NumPy          |
| Database Connectivity | MySQL Connector/Python |
| Visualization         | Microsoft Power BI     |
| Data Source           | CSV / Excel            |
| Version Control       | Git & GitHub           |
| Data Volume           | 50,000+ records        |
| Database Design       | 14 relational tables   |

---

# 🏗️ Project Architecture

The project follows an end-to-end data analytics pipeline:

```text
                RAW DATA
                   │
                   ▼
          CSV / Excel Files
                   │
                   ▼
        ┌─────────────────────┐
        │      Python ETL     │
        │                     │
        │ • Data Cleaning     │
        │ • Transformation    │
        │ • Validation        │
        │ • Error Handling    │
        └─────────────────────┘
                   │
                   ▼
              MySQL DB
                   │
                   ▼
        ┌─────────────────────┐
        │     SQL Analytics   │
        │                     │
        │ • JOINs             │
        │ • Aggregations      │
        │ • Subqueries        │
        │ • CTEs              │
        │ • Indexing          │
        └─────────────────────┘
                   │
                   ▼
          Analytics Dataset
                   │
                   ▼
        ┌─────────────────────┐
        │     Power BI        │
        │                     │
        │ • Data Modeling     │
        │ • DAX Measures      │
        │ • KPIs              │
        │ • Interactive Charts │
        └─────────────────────┘
                   │
                   ▼
          BUSINESS INSIGHTS
                   │
                   ▼
        Data-Driven Decisions
```

---

# 🗄️ Database Design

The backend database is designed using a **normalized relational database structure** consisting of **14 related tables**.

The database demonstrates practical concepts such as:

* Primary Keys
* Foreign Keys
* Relationships between tables
* Normalization
* Referential integrity
* Indexing
* Multi-table JOINs
* Aggregation queries
* Analytical SQL queries
* Query optimization

### Database Workflow

```text
Source Tables
     │
     ├── Customers
     ├── Products
     ├── Orders
     ├── Order Details
     ├── Inventory
     ├── Marketing
     ├── Feedback
     └── Supporting Tables
              │
              ▼
       Relationships
              │
              ▼
       SQL Transformations
              │
              ▼
      Analytics Dataset
```

---

# 🔄 ETL Pipeline

Python is used to automate the data preparation and database-loading process.

## 1. Extract

Raw data is collected from CSV and Excel files.

```text
CSV / Excel
     ↓
Python
     ↓
Pandas DataFrames
```

## 2. Transform

The raw data is cleaned and transformed before loading into MySQL.

Major transformation steps include:

* Handling missing values
* Removing duplicate records
* Correcting data types
* Standardizing column names
* Formatting dates
* Validating numerical fields
* Cleaning categorical values
* Preparing data for relational storage

## 3. Load

The transformed datasets are loaded into MySQL using Python's MySQL connector.

```text
Clean Data
    ↓
Python MySQL Connector
    ↓
MySQL Tables
```

---

# 🐍 Python ETL Automation

The Python pipeline is responsible for automating repetitive data-processing tasks.

### Major Python Responsibilities

```text
Read CSV / Excel
       ↓
Data Validation
       ↓
Missing Value Handling
       ↓
Duplicate Removal
       ↓
Data Transformation
       ↓
Type Conversion
       ↓
Database Connection
       ↓
Bulk Insert / Update
       ↓
Validation & Logging
```

### Libraries Used

```python
import pandas as pd
import numpy as np
import mysql.connector
```

The ETL process is designed to make the workflow repeatable instead of manually importing and cleaning every dataset.

---

# 📊 Power BI Dashboard

The Power BI report is divided into multiple business-focused modules.

---

# 🏠 1. Home Page

The Home page acts as the navigation hub for the dashboard.

### Features

* Project branding
* Business tagline
* Navigation buttons
* Dashboard section access
* Clean and consistent UI
* KPI-oriented design

### Dashboard Preview

![Home Page](https://github.com/user-attachments/assets/ffe80b57-73d3-40c9-8acd-1b4ef551e6c1)

---

# 🌍 2. Business Overview

The Overview page provides a high-level snapshot of the business.

### Key Metrics

* Total Orders
* Total Revenue
* Customer Count
* Revenue Trends
* Inventory Status
* Marketing Performance
* Customer Feedback

This page allows management to quickly understand the overall business situation without navigating through individual reports.

### Dashboard Preview

![Overview](https://github.com/user-attachments/assets/1834e89a-07ea-45cf-8ae8-7175a4e54a01)

---

# 💰 3. Sales Analytics

The Sales Overview page focuses on revenue and order performance.

### Analysis Includes

* Monthly sales
* Yearly sales
* Revenue trends
* Top-performing products
* Area-wise sales
* Payment method analysis
* Customer segments
* Growth analysis

### Business Questions Answered

* Which products generate the highest revenue?
* Which locations generate the most sales?
* How are sales changing over time?
* Which payment methods are most commonly used?
* Which customer segments contribute the most revenue?

### Dashboard Preview

![Sales Overview](https://github.com/user-attachments/assets/8080d5b3-90a2-45d0-828e-7062f7f125a7)

---

# 👥 4. Customer Analytics

The Customer Analytics page focuses on customer behavior and purchasing patterns.

### Analysis Includes

* New customers
* Repeat customers
* Monthly customer growth
* Top customers
* Customer segmentation
* Purchasing behavior

### Business Questions Answered

* How many customers are new vs repeat?
* Are customers returning to purchase again?
* Which customers contribute the most revenue?
* How is the customer base growing?
* Which customer segments are most valuable?

### Dashboard Preview

![Customer Analytics](https://github.com/user-attachments/assets/c8065f34-52a0-4ee4-8b76-5ec7080eb45a)

---

# ⭐ 5. Customer Feedback Analytics

The Feedback Analytics module analyzes customer satisfaction.

### Analysis Includes

* Rating distribution
* Positive feedback
* Neutral feedback
* Negative feedback
* Product quality feedback
* Delivery experience
* Customer satisfaction trends

### Business Questions Answered

* What percentage of customers are satisfied?
* Which products receive poor ratings?
* Are delivery issues affecting customer satisfaction?
* How does customer sentiment change over time?

### Dashboard Preview

![Feedback Analytics](https://github.com/user-attachments/assets/4b29048d-c1d7-4da4-a83d-9d96ee4eec74)

---

# 📦 6. Inventory Analytics

The Inventory Management module helps monitor product availability and stock movement.

### Key Metrics

* Available Stock %
* Damaged Stock %
* Stock Movement
* Reorder Indicators
* Inventory status

### Business Questions Answered

* Which products have low stock?
* Which products may require reordering?
* How much inventory is damaged?
* Which products have high stock movement?
* Where are inventory problems occurring?

### Dashboard Preview

![Inventory Management](https://github.com/user-attachments/assets/9e11e5a3-a294-4a09-b367-7373a4b118ef)

---

# 📢 7. Marketing Analytics

The Marketing Analytics module evaluates campaign performance.

### Key Metrics

* Impressions
* Clicks
* Conversions
* Marketing Spend
* Revenue Generated
* ROI
* Spend vs Profit

### Important Marketing Metrics

**Click-Through Rate**

```text
CTR = Clicks / Impressions × 100
```

**Conversion Rate**

```text
Conversion Rate = Conversions / Clicks × 100
```

**ROI**

```text
ROI = (Revenue - Marketing Spend) / Marketing Spend × 100
```

### Business Questions Answered

* Which campaigns generate the most conversions?
* Which campaigns produce the highest ROI?
* Is marketing spending generating sufficient revenue?
* Which campaigns should receive more budget?

### Dashboard Preview

![Marketing Analytics](https://github.com/user-attachments/assets/4da7fbb9-3d1d-4545-b3f1-b8128b5aba6)

---

# 🧮 SQL Analytics

SQL is used extensively to transform relational data into business-ready information.

The project demonstrates:

### Basic SQL

* SELECT
* WHERE
* ORDER BY
* GROUP BY
* HAVING
* DISTINCT

### Intermediate SQL

* INNER JOIN
* LEFT JOIN
* RIGHT JOIN
* Multiple-table JOINs
* Aggregate functions
* CASE statements
* Subqueries

### Advanced SQL

* CTEs
* Window Functions
* Ranking
* Running totals
* Percentage calculations
* Date-based analysis
* Query optimization
* Indexing

### Example Business Query

```sql
SELECT
    p.product_name,
    SUM(od.quantity * od.unit_price) AS revenue
FROM order_details od
JOIN products p
    ON od.product_id = p.product_id
GROUP BY p.product_name
ORDER BY revenue DESC;
```

This type of query can be used to identify the highest-revenue products.

---

# ⚡ Query Optimization

Performance optimization was considered while designing the database and analytical queries.

### Optimization Techniques

* Indexing frequently queried columns
* Optimizing JOIN conditions
* Avoiding unnecessary columns
* Filtering data before aggregation
* Using appropriate data types
* Reducing unnecessary table scans
* Creating analytics-ready datasets where appropriate

The project achieved an observed **~35% reduction in query execution time** during optimization testing.

> Performance improvement depends on the query, dataset, indexes, and execution environment.

---

# 📈 Key Business KPIs

The dashboard focuses on several important retail KPIs.

| KPI                  | Purpose                                   |
| -------------------- | ----------------------------------------- |
| Total Revenue        | Measures overall sales performance        |
| Total Orders         | Measures transaction volume               |
| Average Order Value  | Measures average customer spend per order |
| Customer Count       | Measures customer base                    |
| Repeat Customer Rate | Indicates customer retention              |
| Conversion Rate      | Measures marketing effectiveness          |
| CTR                  | Measures campaign engagement              |
| Marketing ROI        | Measures campaign profitability           |
| Available Stock %    | Measures inventory availability           |
| Damaged Stock %      | Measures inventory loss                   |
| Average Rating       | Measures customer satisfaction            |

---

# 📐 Example DAX Measures

Power BI measures can be created using DAX.

### Total Revenue

```DAX
Total Revenue =
SUM(OrderDetails[Revenue])
```

### Total Orders

```DAX
Total Orders =
DISTINCTCOUNT(Orders[OrderID])
```

### Average Order Value

```DAX
Average Order Value =
DIVIDE(
    [Total Revenue],
    [Total Orders],
    0
)
```

### Conversion Rate

```DAX
Conversion Rate =
DIVIDE(
    SUM(Marketing[Conversions]),
    SUM(Marketing[Clicks]),
    0
)
```

These measures allow the dashboard to dynamically respond to filters and user selections.

---

# 🔗 Data Modeling

The Power BI model connects business entities through relationships.

A simplified conceptual model is:

```text
                    Customers
                       │
                       │
                       ▼
                    Orders
                       │
                       ▼
                 Order Details
                    │      │
                    │      ▼
                    │   Products
                    │      │
                    ▼      ▼
                Payments  Inventory

Customers ───────────► Feedback

Marketing ────────────► Campaign Performance
```

The model enables users to filter and analyze information across different business dimensions.

---

# 🎛️ Dashboard Interactivity

The Power BI report includes interactive features such as:

* Page navigation
* KPI cards
* Interactive charts
* Slicers
* Date filters
* Product filters
* Customer segmentation
* Location-based filtering
* Cross-filtering
* Drill-down analysis

This allows users to move from a high-level business view to more detailed analysis.

---

# 🔍 Business Insights

The dashboard is designed to help answer practical business questions such as:

### Sales

> Which products and locations are generating the most revenue?

### Customers

> Are customers making repeat purchases?

### Inventory

> Which products require attention because of low availability?

### Marketing

> Which campaigns generate the best return on investment?

### Feedback

> What are the major areas affecting customer satisfaction?

### Management

> What areas of the business require immediate attention?

---

# 🚀 End-to-End Workflow

```text
1. Data Collection
       ↓
2. Raw CSV / Excel Files
       ↓
3. Python Data Cleaning
       ↓
4. Data Transformation
       ↓
5. MySQL Database Loading
       ↓
6. SQL Data Analysis
       ↓
7. JOINs & Aggregations
       ↓
8. Analytics Dataset
       ↓
9. Power BI Data Model
       ↓
10. DAX Measures
       ↓
11. Interactive Dashboards
       ↓
12. Business Insights
```

---

# 📁 Suggested Repository Structure

```text
Blinkit-BI-Dashboard/
│
├── data/
│   ├── customers.csv
│   ├── products.csv
│   ├── orders.csv
│   ├── inventory.csv
│   ├── marketing.csv
│   └── feedback.csv
│
├── python/
│   ├── etl.py
│   ├── data_cleaning.py
│   ├── database_loader.py
│   └── requirements.txt
│
├── sql/
│   ├── database_schema.sql
│   ├── table_creation.sql
│   ├── joins.sql
│   ├── analytics_queries.sql
│   └── indexes.sql
│
├── powerbi/
│   └── Blinkit_BI_Dashboard.pbix
│
├── screenshots/
│   ├── home.png
│   ├── overview.png
│   ├── sales.png
│   ├── customers.png
│   ├── feedback.png
│   ├── inventory.png
│   └── marketing.png
│
└── README.md
```

---

# ⚙️ How to Run the Project

## Step 1 — Clone the Repository

```bash
git clone <your-github-repository-url>
cd Blinkit-BI-Dashboard
```

## Step 2 — Install Python Dependencies

```bash
pip install pandas numpy mysql-connector-python openpyxl
```

## Step 3 — Configure MySQL

Create the required database:

```sql
CREATE DATABASE blinkit_analytics;
```

Then execute the database schema scripts located inside the `sql/` directory.

---

## Step 4 — Configure Database Credentials

Update the Python database connection with your local MySQL credentials.

Example:

```python
connection = mysql.connector.connect(
    host="localhost",
    user="root",
    password="YOUR_PASSWORD",
    database="blinkit_analytics"
)
```

> Do not commit passwords or other credentials to GitHub. Use environment variables for production or shared repositories.

---

## Step 5 — Run the ETL Pipeline

```bash
python python/etl.py
```

The ETL process will:

```text
Read source files
      ↓
Clean data
      ↓
Transform data
      ↓
Connect to MySQL
      ↓
Load tables
      ↓
Validate records
```

---

## Step 6 — Open Power BI

Open:

```text
powerbi/Blinkit_BI_Dashboard.pbix
```

Configure the MySQL connection if required and refresh the dataset.

---

# 📊 Dataset

The project uses a simulated retail dataset containing **50,000+ records** distributed across **14 relational tables**.

The dataset represents business entities such as:

* Customers
* Products
* Orders
* Order details
* Inventory
* Marketing campaigns
* Customer feedback
* Payments
* Locations
* Other supporting entities

> This project is intended for educational and portfolio purposes and does not represent Blinkit's internal or proprietary data.

---

# 🧠 Skills Demonstrated

This project demonstrates practical knowledge of:

### SQL

* Relational databases
* Database design
* Normalization
* Primary and foreign keys
* JOINs
* Subqueries
* CTEs
* Window functions
* Aggregations
* Indexing
* Query optimization

### Python

* Pandas
* NumPy
* Data cleaning
* Data transformation
* ETL automation
* MySQL connectivity
* Data validation
* Error handling

### Power BI

* Data modeling
* DAX
* KPI development
* Interactive dashboards
* Slicers
* Data visualization
* Business storytelling

### Data Analytics

* Sales analysis
* Customer analysis
* Inventory analysis
* Marketing analytics
* Feedback analysis
* KPI analysis
* Business decision support

---

# ⚡ Challenges & Solutions

| Challenge                                          | Solution                                 |
| -------------------------------------------------- | ---------------------------------------- |
| Raw data contained inconsistent values             | Applied Python-based cleaning            |
| Multiple datasets needed to be combined            | Designed relational MySQL schema         |
| Complex business analysis required multiple tables | Used SQL JOINs and aggregations          |
| Repetitive data loading                            | Automated using Python ETL               |
| Slow analytical queries                            | Added indexes and optimized queries      |
| Large number of metrics                            | Created reusable Power BI/DAX measures   |
| Multiple business areas needed to be monitored     | Divided dashboard into dedicated modules |

---

# 📈 Performance Improvements

The project includes several performance-oriented practices:

* Indexed high-traffic columns
* Optimized SQL queries
* Reduced unnecessary data processing
* Used structured relational modeling
* Automated data preparation
* Created analytics-ready datasets
* Reduced observed query execution time by approximately **35%** during optimization testing

---

# 🔮 Future Enhancements

The project can be extended into a more production-oriented analytics platform.

### ☁️ Cloud Deployment

Move MySQL infrastructure to:

* AWS RDS
* Azure Database
* Google Cloud SQL

### 🤖 Machine Learning

Add predictive analytics for:

* Sales forecasting
* Demand forecasting
* Customer churn prediction
* Product recommendation
* Inventory demand prediction

### 🔌 Live API Integration

Replace static CSV files with API-based data ingestion.

```text
API
 ↓
Python ETL
 ↓
Cloud Database
 ↓
Power BI
```

### 🔐 Role-Based Access

Implement different dashboard access levels for:

* Management
* Sales teams
* Inventory teams
* Marketing teams
* Analysts

### ⏱️ Automated Data Refresh

Implement scheduled pipelines using cloud services or workflow automation.

---

# 🎓 Learning Outcomes

Through this project, I gained practical experience in building a complete analytics workflow rather than working with visualization alone.

The project helped me understand how:

```text
Raw Data
   ↓
Data Engineering
   ↓
Database
   ↓
SQL Analytics
   ↓
Data Modeling
   ↓
Visualization
   ↓
Business Decision
```

connects together in a real-world Business Intelligence environment.

---

# 💼 Resume Description

### Blinkit Business Intelligence Dashboard | MySQL, Python, Power BI

* Developed an end-to-end **Business Intelligence dashboard** analyzing 50,000+ retail records across 14 relational tables covering sales, customers, inventory, marketing, and feedback.
* Built a **Python-based ETL pipeline** using Pandas, NumPy, and MySQL Connector for data cleaning, transformation, validation, and automated database loading.
* Designed a normalized **MySQL relational database** and implemented multi-table JOINs, CTEs, aggregations, indexing, and query optimization, achieving an observed ~35% reduction in query execution time during testing.
* Created an interactive **Power BI dashboard** with DAX-based KPIs, slicers, drill-downs, and dedicated analytics modules for sales, customer behavior, inventory, marketing ROI, and customer feedback.

---

# 👨‍💻 Author

## Yaswanth Gutha

**Data Analytics | SQL | Python | Power BI | Business Intelligence**

---

# ⭐ Project Highlights

```text
50,000+ Records
      │
      ▼
14 Relational Tables
      │
      ▼
Python ETL Pipeline
      │
      ▼
MySQL Analytics Database
      │
      ▼
SQL Analysis & Optimization
      │
      ▼
Power BI Dashboard
      │
      ▼
Business Insights
```

---

## 📌 Project Status

**Status:** ✅ Completed — Portfolio / Academic Project

**Domain:** Quick-Commerce / Retail Analytics

**Primary Focus:** Business Intelligence & Data Analytics

**Tools:** MySQL · Python · Pandas · NumPy · Power BI · GitHub
