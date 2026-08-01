# OTT Customer Churn Analysis & Retention Strategy

## Executive Summary
In the hyper-competitive OTT subscription landscape, customer retention is critical for sustainable growth. This end-to-end data analytics project identifies high-risk subscribers by integrating and analyzing multi-dimensional datasets encompassing customer demographics, subscription tiers, and support escalations. 

By building a seamless pipeline from a relational SQL database to a Python environment, this project uncovers the behavioral drivers of churn and provides data-backed, actionable retention strategies to minimize Monthly Recurring Revenue (MRR) leakage.

## 🛠️ Tech Stack & Tools
*   **Database:** SQLite (`sqlite3`)
*   **Programming Language:** Python
*   **Data Manipulation:** `pandas`, `numpy`
*   **Data Visualization:** `matplotlib`, `seaborn`
*   **Reporting:** PowerPoint

## 🔍 Project Workflow
1.  **Relational Data Extraction:** Connected Python to an SQLite database (`customer_ch.db`) to query and merge multi-table datasets (Customer, Subscription, and Support tables).
2.  **Data Cleaning & Quality Checks:** Handled missing values, standardized data types (e.g., datetime conversions), and resolved inconsistencies in categorical variables.
3.  **Advanced Feature Engineering:** Created calculated columns to track vital metrics, including `churn_flag`, `customer_age`, `tenure_days`, and dynamic `churn_risk` scoring based on support escalations and contract types.
4.  **Exploratory Data Analysis (EDA):** Utilized aggregations and pivot tables to evaluate churn by plan type, geography, and subscription models.
5.  **Behavioral Visualization:** Built correlation heatmaps and bar charts to visually isolate the primary indicators of customer drop-off.

## 📊 Key Business Insights
*   **Overall Churn & Retention:** The platform currently experiences a **28.57%** churn rate, maintaining a **71.43%** retention rate.
*   **Contract Vulnerability:** Monthly-contract subscribers represent the highest risk, churning at **55.6%**, which is roughly 6.7 times higher than the annual-contract churn rate (8.3%).
*   **Revenue Impact:** High-risk cohorts account for **18%** of total revenue loss, translating to **USD 73.94** in immediate MRR leakage and **USD 2,047** in Customer Lifetime Value (CLTV) erosion.
*   **Support Correlation:** There is a strong positive correlation (0.77) between customer support escalations and final churn, indicating that unresolved service issues are a primary catalyst for cancellation.

## 📂 Repository Structure
*   `churn_analysis.ipynb`: The core Jupyter Notebook containing all SQL queries, data cleaning, feature engineering, and visualization code.
*   `customer_ch.db`: The source SQLite database containing demographic, subscription, and support tables.
*   `exported_churn_data.csv`: The cleaned and aggregated dataset ready for final modeling and visualization.
*   `Data Analytics Project -Churn Analysis Report.pdf`: The final executive presentation outlining business insights and retention recommendations.