# Walmart Data Analysis: End-to-End SQL + Python Project ✨

🔎 Project Overview

![Project Pipeline](https://github.com/najirh/Walmart_SQL_Python/blob/main/walmart_project-piplelines.png)


This project presents a full-cycle data analysis workflow to extract actionable business insights from Walmart's sales data. It combines the power of Python for data cleaning and processing, SQL for structured querying, and a strategic, business-driven approach to problem solving. Ideal for budding data analysts, it emphasizes hands-on practice with data pipelines, real-world queries, and end-to-end implementation.

---
⚙️ Project Workflow

### ✅ 1. Environment Setup
   - **Tools**: VS Code, Python 3.8+, MySQL
   - **Goal**: Create a well-organized workspace to handle development, data, and analysis components seamlessly.

### ✨ 2. Kaggle API Integration
   - **API Setup**: Obtain your Kaggle API token from [Kaggle](https://www.kaggle.com/) by navigating to your profile settings and downloading the JSON file.
   - **Configure Kaggle**: 
      - Place the downloaded `kaggle.json` file in your local `.kaggle` folder.
      - Use the command `kaggle datasets download -d najir0123/walmart-10k-sales-datasets` to pull datasets directly into your project.

### 📂 3. Download Walmart Sales Dataset
   - **Data Source**: Use the Kaggle API to download the Walmart sales datasets from Kaggle.
   - **Dataset Link**: [Walmart Sales Dataset](https://www.kaggle.com/najir0123/walmart-10k-sales-datasets)
   - **Storage**: Save the data in the `data/` folder for easy reference and access.

### ↓ 4. Install Libraries & Load Data
   - **Libraries**: Install necessary Python libraries using:
     ```bash
     pip install pandas numpy sqlalchemy mysql-connector-python
     ```
   - **Loading Data**: Load CSV to Pandas DataFrame for inspection
### 🔍 5. Data Exploration
   - **Goal**: Conduct an initial data exploration to understand data distribution, check column names, types, and identify potential issues.
   - **Analysis**: Use functions like `.info()`, `.describe()`, and `.head()` to get a quick overview of the data structure and statistics.

### 🔧 6. Data Cleaning
   - **Remove Duplicates**: Identify and remove duplicate entries to avoid skewed results.
   - **Handle Missing Values**: Drop rows or columns with missing values if they are insignificant; fill values where essential.
   - **Fix Data Types**: Ensure all columns have consistent data types (e.g., dates as `datetime`, prices as `float`).
   - **Currency Formatting**: Use `.replace()` to handle and format currency values for analysis.
   - **Validation**: Check for any remaining inconsistencies and verify the cleaned data.

### 📊 7. Feature Engineering
   - **Create New Columns**: Calculate the `Total Amount` for each transaction by multiplying `unit_price` by `quantity` and adding this as a new column.
   - **Enhance Dataset**: Adding this calculated field will streamline further SQL analysis and aggregation tasks.

### 📄 8. Load to MySQL Database
   - **Set Up Connections**: Connect to MySQL and PostgreSQL using `sqlalchemy` and load the cleaned data into each database.
   - **Table Creation**: Set up tables in both MySQL and PostgreSQL using Python SQLAlchemy to automate table creation and data insertion.
   - **Verification**: Run initial SQL queries to confirm that the data has been loaded accurately.

### ❓ 9. SQL Analysis & Business Insights
   - **Use MySQL queries to address business goals:**:Key Questions:
      - Which branch/category generates the most revenue?
      - When are sales highest (time/day/city)?
      - Top-selling products?
      - Customer purchase patterns?
      - Profit margin breakdown?
   - **Documentation**: Keep clear notes of each query's objective, approach, and results.

### 📅 10. Documentation & Publishing
   - Document entire process using Markdown or Jupyter
     - The `README.md` file (this document).
     - Jupyter Notebooks (if applicable).
     - SQL query scripts.
     - Data files (if possible) or steps to access them.

---

## 📆 Requirements

- **Python 3.8+**
- **SQL Databases**: MySQL
- **Python Libraries**:
  - `pandas`, `numpy`, `sqlalchemy`, `mysql-connector-python`
- **Kaggle API Key** (for data downloading)

## Getting Started

1. Clone the repository:
   ```bash
   git clone <repo-url>
   ```
2. Install Python libraries:
   ```bash
   pip install -r requirements.txt
   ```
3. Set up your Kaggle API, download the data, and follow the steps to load and analyze.

---

## 📁 Folder Structure

```plaintext
|-- data/               # Original & cleaned datasets
|-- sql_queries/        # SQL queries for analysis
|-- notebooks/          # Jupyter notebooks
|-- README.md           # Documentation
|-- requirements.txt    # Python dependencies
|-- main.py             # Python script to process data
```
---

## 📊 Results & Insights
- Top Categories by sales & profit
- Best Performing Branches
- Customer Patterns: time-based behavior, payment preferences
- Revenue Trends across regions

## 🤺 Future Improvements

- Dashboarding using Power BI or Tableau
- Incorporate more datasets (inventory, returns, etc.)
- Automate ETL workflows

---

## 💼 License

This project is licensed under the MIT License. 

---

## Acknowledgments

- **Data Source**: Kaggle’s Walmart Sales Dataset
- **Inspiration**: Walmart’s business case studies on sales and supply chain optimization.

---
