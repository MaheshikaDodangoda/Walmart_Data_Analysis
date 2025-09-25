# Walmart Data Analysis: Python + SQL Project

## Project Overview

![Project Logo](https://github.com/MaheshikaDodangoda/main/walmart.png)

This project involves analyzing Walmart sales data to extract meaningful insights such as payment trends, category performance, branch efficiency, and revenue patterns. It uses Python for data cleaning and loading, and SQL(MYSQL/PostgreSQL) for querying. The dataset is processed in a Jupyter Notebook, cleaned, and loaded into a database for analysis.

### 1. Installation
- Install Python and set up a virtual environment.
- Install dependencies: pip install -r requirements.txt.
- Download dataset via Kaggle API and place in project folder.
- Set up MySQL database walmart_db.

### 2. Requirements
- Python 3.8+
- SQL Databases: MySQL / PostgreSQL
- - **Python Libraries**:
  - `pandas`, `numpy`, `sqlalchemy`, `mysql-connector-python`, `psycopg2`
- **Kaggle API Key** (for data downloading)
  
### 3. Explore the Data
- **Goal**: Conduct an initial data exploration to understand data distribution, check column names, types, and identify potential issues.
   - **Analysis**: Use functions like `.info()`, `.describe()`, and `.head()` to get a quick overview of the data structure and statistics.
 
### 4. Data Cleaning
   - **Remove Duplicates**: Identify and remove duplicate entries to avoid skewed results.
   - **Handle Missing Values**: Drop rows or columns with missing values if they are insignificant; fill values where essential.
   - **Fix Data Types**: Ensure all columns have consistent data types (e.g., dates as `datetime`, prices as `float`).
   - **Currency Formatting**: Use `.replace()` to handle and format currency values for analysis.
   - **Validation**: Check for any remaining inconsistencies and verify the cleaned data.

### 5. Data Preparation
   - **Create New Columns**: Calculate the `Total Amount` for each transaction by multiplying `unit_price` by `quantity` and adding this as a new column.
   - **Enhance Dataset**: Adding this calculated field will streamline further SQL analysis and aggregation tasks.

### 6. Load Data into MySQL / PostgreSQL
   - **Set Up Connections**: Connect to MySQL and PostgreSQL using `sqlalchemy` and load the cleaned data into each database.
   - **Table Creation**: Set up tables in both MySQL and PostgreSQL using Python SQLAlchemy to automate table creation and data insertion.

### 7. SQL Analysis
   - **Business Problem-Solving**: Write and execute complex SQL queries to answer critical business questions, such as:
     - Revenue trends across branches and categories.
     - Identifying best-selling product categories.
     - Sales performance by time, city, and payment method.
     - Analyzing peak sales periods and customer buying patterns.
     - Profit margin analysis by branch and category.

## Results and Insights
- **Sales Insights**: Key categories, branches with highest sales, and preferred payment methods.
- **Profitability**: Insights into the most profitable product categories and locations.
- **Customer Behavior**: Trends in ratings, payment preferences, and peak shopping hours.
  
---

## Project Structure

```plaintext
|-- data/                     # Raw data and transformed data
|-- sql_queries/              # SQL scripts for analysis and queries
|-- notebooks/                # Jupyter notebooks for Python analysis
|-- README.md                 # Project documentation
|-- requirements.txt          # List of required Python libraries
|-- main.py                   # Main script for loading, cleaning, and processing data
```
---

## Future Enhancements

Possible extensions to this project:
- Interactive dashboard with Power BI or Tableau
- Real-time data integration
- Predictive analytics for sales forecasting
  
---
## Acknowledgments

- **Data Source**: Kaggle’s Walmart Sales Dataset

    
