# Customer Shopping Behavior Analysis

## Overview

This project analyzes customer shopping behavior using transactional retail data. The objective is to uncover customer purchasing patterns, spending behavior, product preferences, and subscription trends through Python, SQL, and Power BI.

The project follows a complete data analytics workflow, including data cleaning, exploratory data analysis (EDA), database analysis, and dashboard development.

---

## Dataset

The dataset contains customer shopping transactions with demographic, purchasing, and behavioral information.

### Dataset Summary

* **Rows:** 3,900
* **Columns:** 18
* **Key Features:**

  * Customer demographics (Age, Gender, Location)
  * Purchase information (Item Purchased, Category, Purchase Amount)
  * Customer behavior (Frequency of Purchases, Previous Purchases)
  * Marketing variables (Discount Applied, Promo Code Used)
  * Subscription status
  * Review ratings and shipping preferences

---

## Tools & Technologies

### Python

* Pandas
* NumPy
* Matplotlib
* Seaborn

### Database

* Microsoft SQL Server (MSSQL)

### Visualization

* Power BI

### Development Environment

* Jupyter Notebook
* SQL Server Management Studio (SSMS)

---

## Project Workflow

### 1. Data Loading

* Imported dataset into Python using Pandas.
* Performed initial exploration using:

  * `df.info()`
  * `df.describe()`
  * Missing value checks

### 2. Data Cleaning

* Identified and handled missing values.
* Imputed missing review ratings using category-level median values.
* Standardized column names using snake_case.
* Created additional analytical features such as:

  * Age Groups
  * Purchase Frequency Categories

### 3. Exploratory Data Analysis (EDA)

Performed analysis to understand:

* Customer demographics
* Spending patterns
* Product popularity
* Subscription behavior
* Purchase frequency trends
* Rating distributions

### 4. SQL Analysis

Loaded the cleaned dataset into Microsoft SQL Server and answered key business questions:

* Revenue by gender
* High-spending discount users
* Top-rated products
* Shipping type comparison
* Subscribers vs non-subscribers analysis
* Discount-dependent products
* Customer segmentation
* Top products by category
* Repeat buyer analysis
* Revenue by age group

### 5. Power BI Dashboard

Created an interactive dashboard to visualize:

* Total Revenue
* Customer Segments
* Revenue by Gender
* Revenue by Age Group
* Subscription Analysis
* Product Performance
* Shipping Preferences
* Customer Purchase Trends

---

## Key Insights

* Certain age groups generated the highest revenue.
* Subscribers showed stronger purchasing behavior than non-subscribers.
* A small group of products contributed significantly to sales performance.
* Shipping preferences influenced customer purchasing decisions.
* Repeat customers represented a valuable segment for retention strategies.

---

## Business Recommendations

* Increase subscription incentives and exclusive offers.
* Develop customer loyalty programs for repeat buyers.
* Optimize discount strategies to balance revenue and profitability.
* Promote top-performing products through targeted campaigns.
* Focus marketing efforts on high-value customer segments.

---

## How to Run

### Python Analysis

1. Clone the repository.
2. Install required libraries:

```bash
pip install pandas numpy matplotlib seaborn pyodbc
```

3. Run the Jupyter Notebook:

```bash
jupyter notebook
```

### SQL Analysis

1. Import the cleaned dataset into Microsoft SQL Server.
2. Execute the SQL scripts provided in the `sql_queries` folder.

### Power BI Dashboard

1. Open the `.pbix` file in Power BI Desktop.
2. Refresh the data source if required.
3. Explore the interactive dashboard.

---

## Project Structure

```text
Customer-Shopping-Behavior-Analysis/
│
├── data/
│   ├── raw_data.csv
│   └── cleaned_data.csv
│
├── notebooks/
│   └── customer_behavior_analysis.ipynb
│
├── sql_queries/
│   └── analysis_queries.sql
│
├── powerbi/
│   └── customer_dashboard.pbix
│
├── images/
│   └── dashboard_screenshot.png
│
└── README.md
```

---

## Author

**Dr. Ifunanya Nze**
Data Analyst | Veterinarian | Public Health Professional

