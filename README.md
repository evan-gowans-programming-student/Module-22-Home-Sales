# Home Sales Analysis

## Overview
This project leverages **Apache Spark** and **PySpark SQL** to analyze home sales data. It provides insights into average home prices based on different criteria and optimizes queries using caching and partitioning.

## Files in this Repository
- **`Home_Sales.ipynb`** – The Jupyter Notebook that performs data analysis on home sales.  
- **`README.md`** – This document explaining how to use the notebook.

## Prerequisites
Before running the notebook, make sure you have:
- Python 3 installed  
- Apache Spark and PySpark installed  
- Jupyter Notebook installed

You can install the required dependencies using:
```bash
pip install findspark pyspark pandas
```

## Instructions to Run the Notebook

### Step 1: Clone the Repository
```bash
git clone https://github.com/evan-gowans-programming-student/Module-22-Home-Sales.git
cd Module-22-Home-Sales
```

### Step 2: Open Jupyter Notebook
Start Jupyter Notebook from the terminal:
```bash
jupyter notebook
```
Then, open `Home_Sales.ipynb`.

### Step 3: Run Each Cell
Execute each cell in sequential order. The notebook will process home sales data, analyze trends, and optimize performance.

### Step 4: Generate Parquet File
The notebook automatically creates a new Parquet file when executed. Ensure the directory has write permissions for proper file creation.

## Features in the Notebook
- Loads home sales data from an AWS S3 bucket  
- Creates a Spark DataFrame and a temporary SQL table  
- Executes SQL queries to compute average home prices based on various attributes  
- Uses caching to improve query performance  
- Implements data partitioning for efficient data storage  

## Expected Output
- Query results showing home price trends  
- Comparison of query run times for cached vs. uncached data  
- A dynamically created Parquet file, eliminating manual storage issues  

## Notes
If `findspark` or `pyspark` isn’t working, reinstall them using:
```bash
pip install findspark pyspark
```

If a Parquet file already exists, run the notebook to generate a fresh one.  
Restart the kernel if any package/module errors occur.
