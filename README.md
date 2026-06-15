# Customer Shopping Behavior Analysis
### A Data Analytics Portfolio Project | Python • SQL Server • Power BI

---

## Overview

How do customers shop, and what can a business do about it?

This project analyses 3,900 customer transactions to uncover patterns in buying behavior, product performance, shipping preferences, and customer loyalty. The goal is to help businesses make smarter marketing and operational decisions based on real data — not guesswork.

---

## Dataset

- **Source:** Customer Shopping Behavior Dataset (Kaggle)
- **Rows:** 3,900 transactions
- **Format:** CSV/Excel
- **Key columns:** Age, Gender, Item Purchased, Category, Purchase Amount, Review Rating, Subscription Status, Discount Applied, Shipping Type, Frequency of Purchases

---

## Tools Used

| Tool | Purpose |
|---|---|
| Python (Pandas, NumPy) | Data loading, cleaning, feature engineering |
| SQL Server (SSMS) | Business queries and data exploration |
| SQLAlchemy + PyODBC | Python to SQL Server connection |
| Power BI | Dashboard and visualisation |

---

## Steps

### 1. Data Loading & Inspection
- Loaded dataset into Python using Pandas
- Inspected shape, data types, null values, and duplicates
- Identified columns needing transformation

### 2. Data Cleaning
- Handled missing values using median imputation per product category for Review Rating
- Standardised categorical columns
- Validated data types across all columns

### 3. Feature Engineering
- Created `age_group` column by binning ages into: Young Adults, Adults, Middle Aged, Senior
- Created `frequency_of_purchases_days` to convert purchase frequency labels into numeric values

### 4. Database Integration
- Connected Python to Microsoft SQL Server using SQLAlchemy and PyODBC
- Pushed cleaned dataframe into SQL Server database (`customer_behavior`)
- Queried data directly from SQL Server for business analysis

### 5. SQL Business Analysis
Wrote 10 business queries to answer key questions:

| # | Question | Finding |
|---|---|---|
| 1 | Which gender buys more? | Males purchase more than females |
| 2 | Do discount buyers spend more? | Yes — discount buyers transact more |
| 3 | Top 5 rated products? | Gloves (3.86), Sandals (3.84), Boots (3.82), Hat (3.80), Skirt (3.78) |
| 4 | Which shipping type generates most revenue? | Express shipping leads in revenue |
| 5 | Do subscribers buy more? | No — non-subscribers purchase more |
| 6 | Top 5 discounted products? | Socks, Blouse, Sandals, Skirt, Handbag |
| 7 | How loyal are customers? | Business has strong loyal customer base |
| 8 | Who repeat-purchases more? | Non-subscribers repeat more than subscribers |
| 9 | Which age group buys most? | Young Adults lead in purchases |
| 10 | Revenue by customer segment? | Analysed across age, gender, and subscription status |

### 6. Power BI Dashboard
- Connected Power BI directly to SQL Server database
- Built interactive single-page dashboard with slicers and charts

---

## Dashboard

**KPI Cards:**
- Total Customers: 3,900
- Average Review Rating: 3.75
- Average Revenue: $59.8M

**Visuals:**
- Pie chart — Subscribers vs Non-subscribers
- Clustered bar — Revenue by Category
- Clustered bar — Sales by Category
- Clustered column — Revenue by Age Group
- Clustered column — Sales by Age Group

**Slicers:**
- Subscription Status
- Gender
- Category
- Shipping Type

---

## Key Results & Recommendations

1. **Target male customers** — they drive more purchases and should be prioritised in campaigns
2. **Expand discount strategy** — discount buyers transact more frequently; a structured promo calendar could increase revenue
3. **Invest in Express shipping** — it generates the most revenue; consider making it the default or promoting it as a value-add
4. **Re-evaluate subscription model** — non-subscribers outperform subscribers in both volume and repeat purchases; promote exclusive benefits for subscribers
5. **Focus on Young Adults** — they are the highest-spending age group and should anchor your marketing strategy
6. **Protect top-rated products** — Gloves, Sandals, and Boots have the highest ratings; ensure consistent stock and visibility
6. **Customer Loyalty Programs** – Reward repeat buyers to move them into Loyal customers


---

## How to Run

### Python
```bash
# Install dependencies
pip install pandas numpy sqlalchemy pyodbc openpyxl

# Run the notebook
jupyter notebook Customer_Shopping_Behavior_Analysis.ipynb
```

### SQL
- Open SQL Server Management Studio (SSMS)
- Connect to your server
- Run queries from `queries.sql`

### Power BI
- Open `Customer_Shopping_Dashboard.pbix`
- Update the SQL Server connection to your server name
- Refresh data

---

## Project Structure

```
customer-shopping-behavior-analysis/
│
├── Customer_Shopping_Behavior_Analysis.ipynb  # Python notebook
├── queries.sql                                 # All 10 SQL queries
├── Customer_Shopping_Dashboard.pbix           # Power BI file
├── customer_shopping_behavior.xlsx            # Raw dataset
├── Report.docx                                # Full analysis report
└── README.md                                  # This file
```

---

## Author

**Dr. Ifunanya Grace Nze**
Veterinarian | Data Analyst | AI & Automation Consultant

> *"Turning messy data into business decisions."*

---
