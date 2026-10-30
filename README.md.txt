# Python Retail Data Cleaning and Sales Analysis

## Project Overview

This project demonstrates data cleaning, data quality assessment,
sales analysis, and data visualization using Python.

I analyzed a sample of 10,000 transaction records from the
UCI Online Retail dataset using Pandas, Matplotlib, and Seaborn.

After cleaning, 9,658 valid sales records remained.

The project includes:
- Automated data quality assessment
- Data cleaning using Python and Pandas
- Before-and-after data quality comparison
- Sales performance analysis
- Product and country rankings
- Five professional data visualizations

## Tools and Skills

**Languages:** Python

**Libraries:** Pandas, NumPy, Matplotlib, Seaborn

**Environment:** Google Colab

**Skills demonstrated:**
- Data cleaning
- Duplicate detection
- Missing-value analysis
- Data validation
- Data transformation
- Sales analysis
- Data visualization
- Reproducible analysis using Jupyter notebooks

## Dataset

**Source:** UCI Machine Learning Repository

**Dataset:** Online Retail

**Dataset link:**
https://archive.ics.uci.edu/dataset/352/online+retail

The original dataset contains approximately 541,909 rows.

This project uses the first 10,000 transaction rows.

The analyzed sample covers December 2010.

## Data Cleaning Results

| Data Quality Metric | Before | After |
|---|---:|---:|
| Total Records | 10,000 | 9,658 |
| Missing Customer IDs | 2,291 | 2,246 |
| Missing Descriptions | 42 | 0 |
| Cancelled Transaction Rows | 100 | 0 |
| Invalid Quantities | 130 | 0 |
| Invalid Prices | 46 | 0 |
| Duplicate Records | 196 | 0 |

**342 rows removed (3.42%).**

**9,658 rows retained (96.58%).**

Missing Customer IDs were retained because these records
could still represent valid sales.

## Sales Performance KPIs

| KPI | Result |
|---|---:|
| Total Sales | £183,529.13 |
| Total Units Sold | 89,731 |
| Unique Invoices | 424 |
| Average Sales per Invoice | £432.85 |

## Key Business Insights

### 1. Sales by Country

The United Kingdom generated **£167,651.80**,
representing approximately **91.35%** of total sales.

### 2. Highest-Revenue Product

**REGENCY CAKESTAND 3 TIER**

Sales: **£7,717.95**

### 3. Highest-Volume Product

**WORLD WAR 2 GLIDERS ASSTD DESIGNS**

Units sold: **3,409**

### 4. Monthly Sales

The sample covers **December 2010**.

Total sales: **£183,529.13**.

Because the sample contains only one month,
monthly sales comparisons were not possible.

## Visualizations

### Data Quality Before and After Cleaning

![Data Quality Comparison](charts/data_quality_comparison.png)

### Top 10 Products by Sales

![Top Products by Sales](charts/top_products_sales.png)

### Top 10 Products by Quantity

![Top Products by Quantity](charts/top_products_quantity.png)

### Sales by Country

![Sales by Country](charts/sales_by_country.png)

### Monthly Sales

![Monthly Sales](charts/monthly_sales.png)

## Project Files

- [Python Notebook](notebooks/retail_data_cleaning.ipynb)
- [Cleaned Dataset](results/cleaned_retail_data.csv)
- [Data Quality Report](results/data_quality_report.csv)
- [Top 10 Products by Sales](results/top_10_products_sales.csv)
- [Top 10 Products by Quantity](results/top_10_products_quantity.csv)
- [Sales by Country](results/sales_by_country.csv)
- [Monthly Sales](results/monthly_sales.csv)
- [Business Insights Report](reports/business_insights.md)

## Comparison With Excel Project

This project cleaned the same 10,000-row retail sample
as my Excel project.

Both tools produced identical results:

| KPI | Excel | Python |
|---|---:|---:|
| Cleaned Records | 9,658 | 9,658 |
| Total Sales | £183,529.13 | £183,529.13 |
| Total Units Sold | 89,731 | 89,731 |
| Unique Invoices | 424 | 424 |
| Average Sales per Invoice | £432.85 | £432.85 |

This confirms that both cleaning processes
produced consistent results.

## Limitations

- Only 10,000 rows from the original dataset were analyzed.
- The sample covers December 2010 only.
- Cancelled transactions were excluded.
- Sales represent positive sales, not net revenue after returns.
- Missing Customer IDs were retained.
- Results should not be generalized to the full dataset.

## Conclusion

This project demonstrates how Python can be used to
automate data cleaning, assess data quality, analyze sales
performance, and create professional visualizations.

Together with my SQL and Excel projects, this demonstrates
practical Data Analyst skills across three tools:

- **SQL** for database querying and business analysis
- **Excel** for data cleaning, PivotTables, and dashboards
- **Python** for automated cleaning, analysis, and visualization