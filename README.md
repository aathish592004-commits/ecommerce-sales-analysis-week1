# E-Commerce Sales Analysis – Data Science Internship, Week 1

**Organization:** WeIntern Pvt Ltd
**Week 1 objective:** Build data cleaning and analytical thinking skills through data cleaning, KPI analysis, visualization and reporting.

## Project Summary

This project cleans the Online Retail transaction dataset, calculates core sales KPIs, analyses sales trends and customer behaviour, and presents the results in charts, a Power BI dashboard and a written report.

## Dataset Description

- **Source:** Online Retail.xlsx (transactions of a UK-based online gift retailer)
- **Period:** 1 Dec 2010 to 9 Dec 2011
- **Raw size:** 541,909 rows × 8 columns
- **Columns:** InvoiceNo, StockCode, Description, Quantity, InvoiceDate, UnitPrice, CustomerID, Country
- **Derived column:** Revenue = Quantity × UnitPrice
- **Cleaned size:** 524,878 rows, 19,960 orders, 4,338 identified customers, 38 countries

Note: the dataset has no Category, payment mode or delivery status columns, so the Top-Selling Category KPI could not be calculated.

## Tools and Libraries

- Python 3 (pandas, NumPy, Matplotlib, Seaborn, openpyxl)
- Jupyter Notebook
- Power BI Desktop

## Key Steps Performed

1. **Inspection:** reviewed shape, data types, summary statistics and missing values.
2. **Duplicates:** found and removed 5,268 fully duplicated rows. Repeated invoice numbers were kept, since one invoice holds many product lines.
3. **Missing values:** removed 1,454 rows with no Description (0.27%). Rows with no CustomerID (24.9%) were kept for sales analysis and excluded only from customer-level analysis.
4. **Validation:** converted InvoiceDate to datetime, then kept only rows with Quantity > 0, UnitPrice > 0 and invoice numbers not starting with "C" (cancellations).
5. **Feature creation:** added the Revenue column.
6. **Analysis:** calculated KPIs, monthly trends, country, product and customer breakdowns, and outlier checks.
7. **Visualization:** built Matplotlib/Seaborn charts and a Power BI dashboard.
8. **Reporting:** wrote the final report with findings and recommendations.

## Major Findings

- Total revenue is **£10.64M** from **19,960 orders**, with an average order value of **£533.17** and **5.57M units** sold (currency assumed GBP).
- **September to November 2011** earned about 35% of revenue; November was the peak at £1.50M.
- The **United Kingdom** provides 84.6% of revenue.
- **Repeat customers** make up 65.6% of identified customers and generate 93.1% of identified-customer revenue.
- The top 20% of customers drive about 75% of revenue.
- Shipping and adjustment lines (DOTCOM POSTAGE, POSTAGE, Manual) and two bulk orders (invoices 581483 and 541431) distort product and trend charts and should be treated with care.

## Folder Structure

```
data-science-week1-assignment/
├── data/
│   ├── raw/                  # Online Retail.xlsx (unchanged)
│   └── cleaned/              # online_retail_cleaned.csv
├── notebooks/
│   └── week1_analysis.ipynb
├── outputs/
│   ├── charts/
│   └── dashboard/
├── reports/
│   └── final_report.pdf
├── screenshots/
├── README.md
└── requirements.txt
```

## Execution Instructions

1. Clone the repository and open a terminal in its root folder.
2. Install the requirements:
   ```
   pip install -r requirements.txt
   ```
3. Place `Online Retail.xlsx` in `data/raw/`.
4. Open `notebooks/week1_analysis.ipynb` in Jupyter and run all cells from top to bottom. The cleaned dataset is saved to `data/cleaned/` and charts to `outputs/charts/`.
5. Open the Power BI dashboard from `outputs/dashboard/`, or view the screenshot in `screenshots/`.

## Author

**Athish M**
MCA Student, Alliance University, Bangalore
