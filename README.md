# 📊 Retail Sales & Customer Analytics using PySpark

An advanced data analytics project built with **Apache Spark (PySpark)** to extract actionable business intelligence from retail sales data. This repository contains a comprehensive notebook (`pyspark_retail_analysis.ipynb`) that demonstrates proficiency in distributed data processing, complex Spark SQL transformations, and advanced PySpark functions.

## 🛠️ Tech Stack
* **Processing Engine:** Apache Spark (PySpark)
* **Environment:** Databricks / Local Jupyter Notebooks
* **Language:** Python / Spark SQL
* **Data Structures:** Spark DataFrames

## 💡 What's Inside the Notebook?

This project simulates a real-world analytics workflow, solving complex business questions across four key domains:

### 1. Sales & Regional Performance
* **Revenue Calculations:** Engineered features to calculate total transaction amounts and aggregated monthly sales summaries.
* **Pivot Tables:** Dynamically pivoted product categories against regional data to create a comprehensive cross-tabulated revenue matrix.
* **Top Performers:** Identified the top 3 best-selling products by total revenue across the dataset.

### 2. Customer Insights & Segmentation
* **Distributed Percentile Calculation:** Utilized PySpark's highly optimized `approxQuantile` method to segment customers into High, Medium, and Low-value tiers based on total spend, avoiding single-node execution bottlenecks.
* **Purchase Frequency:** Leveraged `Window.partitionBy` and `lag()` functions to calculate the average number of days between customer purchases.

### 3. Store Performance & Product Analytics
* **Store Metrics:** Calculated total sales, number of unique customers, and true average sale per customer (with division-by-zero handling) for every store.
* **Inventory Insights:** Analyzed inventory movement to identify slow-moving products (bottom 10% of total sales volume) to inform supply chain strategies.

### 4. Supplier Reliability
* **Correlated Subqueries:** Executed advanced Spark SQL queries to identify suppliers whose reliability scores fell below the global average.
* **Weighted Averages:** Calculated delivery reliability scores weighted against total product revenue to prioritize high-impact supplier relationships.

## 🚀 How to View & Run
1. You can view the code directly here on GitHub by clicking on the `pyspark_retail_analysis.ipynb` file.
2. To run it yourself, clone this repository or download the `.ipynb` file.
3. Import the notebook into a Databricks Workspace or run it via a local Jupyter Notebook with PySpark installed.
