# Customer Analysis – Online Retail Dataset

## Overview
This project analyzes customer purchasing behavior for an online retail store using Python.  
The goal is to identify top customers, understand country-level revenue patterns, and uncover monthly sales trends to support data-driven business decisions.

---

## Project Structure
```
Online-Retail-Analysis/
│
├── data/
│   └── OnlineRetail.xlsx          # Raw dataset
│
├── code/
│   └── 	OnlineRetailAnalsis.ipynb       # Python analysis script
│
└── README.md
```

---

## Data Cleaning
- Removed rows with missing `CustomerID` or `Description`.
- Filtered out negative or zero quantities and prices.
- Converted `InvoiceDate` to datetime.
- Created `Year` and `Month` columns for time-series analysis.

---

## Features and Metrics
A customer-level dataset (**CustomerProfile**) was created with the following metrics:

- TotalSpent – total amount spent by each customer  
- TotalQuantity – total quantity of products purchased  
- NumInvoices – number of unique purchase invoices  
- AvgQuantityPerInvoice  
- AvgPurchaseAmount

Additional analyses include:

- Revenue by country  
- Unique customers by country  
- Monthly sales analysis  
- Top 10 customers by spending, quantity, and invoices  
- Distribution charts for spending and quantities  

---

## Visualizations
The project includes several visualizations created with Matplotlib and Seaborn:

- Top 10 customers by total spending  
- Top 10 customers by total quantity  
- Revenue by country  
- Monthly sales trends  
- Distribution of customer spending  
- Distribution of average quantities  

All charts are in English, with explanatory Hebrew comments in the code.

---

## Key Insights
- The UK is the largest and most profitable market.  
- Some countries generate high revenue despite having fewer customers (e.g., Netherlands).  
- Seasonal demand peaks in October–November.  
- Customer behavior varies significantly: some customers spend a lot in few purchases, others buy many invoices with lower quantities.

---

## Business Recommendations
- Create tailored loyalty offers for high-spending customers.  
- Strengthen marketing activities in the UK, Germany, and the Netherlands.  
- Run campaigns aligned with peak sales months.  
- Develop product bundles for customers who purchase large quantities.  
- Identify and retain high-value returning customers.

---

## Technologies Used
- Python: Pandas, Matplotlib, Seaborn  
- Excel (raw dataset)  
- Google Colab / Jupyter Notebook

---

## Included Files
- `OnlineRetail.xlsx` – raw dataset  
- `	OnlineRetailAnalsis.ipynb` – full analysis script  
