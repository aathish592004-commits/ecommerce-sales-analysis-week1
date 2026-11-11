# E-Commerce Sales Analysis – Data Science Internship, Week 1

**Organization:** WeIntern Pvt Ltd  
**Author:** Athish M  
**Program:** MCA – Data Science  
**Tools:** Python, Pandas, Jupyter Notebook, Power BI

## Project Objective

The objective of this project is to develop data cleaning and analytical skills by examining an e-commerce transaction dataset, calculating key performance indicators (KPIs), identifying sales trends and presenting insights through visualizations and a Power BI dashboard.

## Project Summary

This project analyses the Online Retail transaction dataset of a UK-based online gift retailer. It includes data preprocessing, sales KPI calculations, monthly revenue analysis, product performance analysis, country-wise revenue analysis and dashboard development.

## Dataset Description

- **Dataset:** Online Retail.xlsx
- **Source:** UCI Machine Learning Repository
- **Period:** 1 December 2010 – 9 December 2011
- **Original size:** 541,909 rows × 8 columns
- **Cleaned size:** 524,878 rows
- **Orders:** 19,960
- **Identified customers:** 4,338
- **Countries:** 38

**Derived column:** Revenue = Quantity × UnitPrice.

**Dataset limitation:** The dataset does not contain a Category column. Therefore, the Top-Selling Category KPI could not be calculated.

## Tools and Technologies

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Jupyter Notebook
- Power BI Desktop
- Excel

## Data Cleaning and Preparation

1. Inspected the dataset structure, data types and missing values.
2. Identified and removed 5,268 duplicate rows.
3. Removed rows with missing product descriptions.
4. Retained records with missing CustomerID for overall sales analysis.
5. Converted InvoiceDate into datetime format.
6. Removed cancelled transactions and invalid quantity or price records.
7. Created a Revenue column using Quantity × UnitPrice.

## Key Performance Indicators

| KPI | Result |
|---|---:|
| Total Revenue | £10,642,110.80 |
| Total Orders | 19,960 |
| Average Order Value | £533.17 |
| Total Units Sold | 5,572,420 |

## Major Findings

- Total revenue reached approximately £10.64 million.
- November 2011 recorded the highest monthly revenue, approximately £1.50 million.
- The United Kingdom contributed approximately 84.6% of total revenue.
- September to November 2011 represented a strong revenue period.
- Product performance varied significantly across the top-selling products.
- Postage and manual adjustment entries should be considered when interpreting product revenue rankings.

## Visualizations

The project includes:

- Monthly Revenue Trend – Line Chart
- Top 10 Products by Revenue – Bar Chart
- Revenue Share by Country – Pie Chart
- Revenue Distribution – Chart
- Correlation Heatmap
- Power BI Sales Dashboard

## Power BI Dashboard

The interactive dashboard presents:

- Total Revenue
- Total Orders
- Average Order Value
- Total Units Sold
- Monthly Revenue Trend
- Top 10 Products by Revenue
- Revenue Share by Country

## Repository Contents

| File | Description |
|---|---|
| `week1_analysis.ipynb` | Python analysis and data cleaning |
| `Online Retail.xlsx` | Original dataset |
| `online_retail_cleaned.zip` | Compressed cleaned dataset |
| `Ecommerce_Sales_Analysis.pbix` | Power BI dashboard |
| `E-Commerce Sales Analysis – Final Report.pdf` | Final project report |
| `kpi_summary.csv` | KPI summary |
| `monthly_revenue.png` | Monthly revenue visualization |
| `revenue-share-by-country-pie.png` | Country-wise revenue visualization |
| `revenue_distribution.png` | Revenue distribution visualization |
| `correlation_heatmap.png` | Correlation heatmap |
| `dashboard-mockup.png` | Dashboard mockup |
| `requirements.txt` | Python dependencies |

## How to Run

1. Clone or download this repository.
2. Install the required Python libraries:

```bash
pip install -r requirements.txt
```

3. Open `week1_analysis.ipynb` using Jupyter Notebook.
4. Run the notebook cells in sequence.
5. Open `Ecommerce_Sales_Analysis.pbix` using Power BI Desktop to explore the dashboard.

## Conclusion

This project demonstrates practical skills in data cleaning, exploratory data analysis, KPI calculation, data visualization and business reporting using Python and Power BI.

---

**Author:** Athish M  
**Project:** WeIntern Data Science Internship – Week 1
