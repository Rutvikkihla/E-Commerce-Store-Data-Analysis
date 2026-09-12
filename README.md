# 🛒 E-commerce Superstore Sales & Profit Analysis
 
A complete end-to-end data analytics project analyzing **9,994 retail transactions** across the United States — uncovering monthly sales trends, category performance, profit drivers, and customer segment insights using Python and interactive Plotly visualizations.

## 📌 Overview
This project analyzes the Superstore retail dataset to answer real business questions around sales performance, profit margins, product category trends, and customer segment behavior. The analysis covers the full analytics workflow — from raw data loading and cleaning to feature engineering and interactive visual storytelling.

## 🎯 Business Questions:
1. Which month has the highest and lowest sales?:
2. Which product category has the highest and lowest sales?:
3. Which sub-categories contribute the most and least sales?:
4. Which month has the highest profit?:
5. Which categories and sub-categories are most and least profitable?:
6. Which customer segment generates the highest sales and profit?:
7. What is the Sales / Profit ratio for each customer segment?:

## 📂 Dataset
 
| Property | Details |
|---|---|
| **Rows** | 9,994 |
| **Columns** | 21 |
| **Date Range** | 2017 |
| **Geography** | United States — 49 States, 4 Regions |
| **File** | `Superstore.csv` |

## Main Fields 
| Field | Description |
|---|---|
| **Order ID** | Order identifier |
| **Order Date** | Order date |
| **Ship Date** | Shipment date |
| **Ship Mode** | Shipping method |
|**Customer ID**|Customer identifier|
|**Customer Name**|Customer name|
|**Segment**|Customer segment|
|**Country, City, State, Region**|Geographic dimensions|
|**Product ID**|Product identifier|
|**Category**|Product category|
|**Sub-Category**|Product sub-category|
|**Product Name**|Product name|
|**Sales**|Sales amount|
|**Quantity**|Units sold|
|**Discount**|Applied discount|
|**Profit**|Profit amount|

**Tools & Technologies:** `Order Date`,
`Python` ,`Pandas`, `Plotly Express`, `Plotly Graph Objects`, `Jupyter Notebook`, `CSV`

## 🔄 Project Workflow
 
### 1 — Data Loading & Exploration
- Loaded dataset using `pandas` with Latin-1 encoding
- Explored structure using `df.info()` and `df.describe()`
- Identified column types, value ranges, and null values
### 2 — Data Cleaning & Feature Engineering
- Converted `Order Date` and `Ship Date` to datetime format
- Engineered new time-based features:
  - `order_month` — extracted month from Order Date
  - `order_day_of_week` — extracted weekday from Order Date
  - `order_year` — extracted year from Order Date
- Exported cleaned dataset as `Clean_Superstore.csv`
### 3 — Exploratory Data Analysis (10 Business Questions)
 
| # | Analysis |
|---|---|
| Q1 | Monthly Sales Analysis — best and worst performing months |
| Q2 | Sales by Category — which category leads in revenue |
| Q3 | Sales by Sub-Category — granular product performance |
| Q4 | Monthly Profit Analysis — profit trends across the year |
| Q5 | Profit by Category — which categories are truly profitable |
| Q6 | Profit & Loss by Sub-Category — identifying loss-making products |
| Q7 | Sales & Profit by Customer Segment — Consumer vs Corporate vs Home Office |
| Q8 | Sales-to-Profit Ratio by Segment — efficiency of each customer group |
 
### 4 — Visualizations Built
- 📈 Line chart — Monthly sales trend
- 🍩 Donut charts — Sales and profit share by category
- 📊 Bar charts — Sub-category sales, monthly profit, segment comparison
- 📊 Grouped bar chart — Sales vs profit side-by-side by segment
---
 
## 📈 Key Results
 
| Insight | Finding |
|---|---|
| **Total Sales** | $2,297,201 |
| **Total Profit** | $286,397 |
| **Profit Margin** | 12.47% |
| **Total Orders** | 5,009 |
| **Total Customers** | 793 |
| **Average Order Value** | $458.61 |
| **Best Sales Month** | November ($352,461) |
| **Worst Sales Month** | February ($59,751) |
| **Best Profit Month** | December ($43,369) |
| **Top Category by Sales** | Technology ($836,154) |
| **Top Sub-Category by Profit** | Copiers ($55,618) |
| **Loss-Making Sub-Category** | Tables (−$17,725), Bookcases (−$3,473) |
| **Top Customer Segment** | Consumer ($1.16M sales, $134K profit) |
| **Most Efficient Segment** | Home Office (lowest Sales-to-Profit ratio) |
| **Most Profitable Region** | West ($108,418) |
| **Least Profitable Region** | Central ($39,706) |

## Customer Segments
|Segment|Sales|Profit|Sales / Profit (Ratio)|
|---|---|---|---|
|Consumer|$1,161,401.00|$134,119.21|8.66|
|Corporate|$706,146.40|$91,979.13|7.68|
|Home Office|$429,653.10|$60,298.68|7.13|

---
## Business Insights

**1. Seasonal Sales Pattern** - Sales are strongest toward the end of the year, with November as the highest-sales month in the notebook results.

**2. Technology Leadership** - Technology is the strongest category for both sales and aggregate profit.

**3. Product Performance Difference** - Phones leads sub-category sales, while Copiers leads sub-category profit.

**4. Profitability Risk Areas** - Tables, Bookcases, and Supplies show negative aggregate profit and deserve deeper investigation.

**5. Customer Segment Contribution** - Consumer customers contribute the largest sales and profit totals.

**6. Revenue Is Not the Whole Story** - Sales performance alone can hide profitability problems; sub-category profit analysis highlights areas where revenue does not translate into positive profit.

---
 
## 💡 Business Recommendations
 
- **Discontinue or reprice Tables** — Running at a loss of $17,725; high discounting is likely the cause; review discount policy immediately
- **Push Copiers and Phones** — Top profit contributors; prioritize these in marketing campaigns and inventory stocking
- **November promotions** — Peak sales month; double down with targeted campaigns to maximize revenue
- **Boost February sales** — Worst performing month; consider early-year discount events or loyalty offers to lift sales
- **Focus on Consumer segment** — Highest revenue and profit contributor; personalized campaigns can deepen retention
- **Investigate Central region** — Lowest profit despite decent sales; likely high discount or high return rates to investigate
- `Inventory Planning` → Prepare capacity for strong November–December demand.
-`Profitability Review` → Investigate pricing, discounts, and product economics for loss-making sub-categories.
-`KPI Monitoring` → Track sales and profit together instead of relying only on revenue.
-`Deeper Analysis` → Add regional and product-level diagnostics to understand profitability drivers.
---
 
## 📁 Repository Structure
 
```
📦 Superstore-Sales-Analysis
 ┣ 📓 Main.ipynb                  # Full EDA notebook with visualizations
 ┣ 📄 Superstore.csv              # Raw dataset
 ┣ 📄 Clean_Superstore.csv        # Cleaned dataset (output)
 ┗ 📖 README.md
```

## 🚀 How to Run
 
**Prerequisites**
```
Python 3.8+
Required libraries: pandas, plotly, jupyter
```
 
**Steps**
 
```bash
# 1. Clone the repository
git clone https://github.com/Rutvikkihla/Superstore-Sales-Analysis.git
cd Superstore-Sales-Analysis
 
# 2. Install dependencies
pip install pandas plotly jupyter
 
# 3. Launch the notebook
jupyter notebook Main.ipynb
```

