# Customer Analysis – Online Retail Dataset

## Overview
This project analyzes customer purchasing behavior for an online retail store using Python.  
The goal is to identify top customers, understand country-level revenue patterns, and uncover monthly sales trends to support data-driven business decisions.

---

## Dataset Source
The dataset used in this project was obtained from Kaggle:  
[Online Retail Dataset – Kaggle](https://www.kaggle.com/datasets/ulrikthygepedersen/online-retail-dataset)

---

## Project Structure
```
Online-Retail-Analysis/
│
├── code/
│   └── OnlineRetailAnalysis.ipynb     # Python analysis notebook
│
└── README.md
```

---

## Data Cleaning
- Removed rows with missing `CustomerID` or `Description`  
- Filtered out negative or zero quantities and prices  
- Converted `InvoiceDate` to datetime format  
- Created `Year` and `Month` columns for time-series analysis  

---

## Features and Metrics
A customer-level dataset (**CustomerProfile**) was created with the following metrics:

- **TotalSpent** – total amount spent by each customer  
- **TotalQuantity** – total quantity of items purchased  
- **NumInvoices** – number of unique purchase invoices  
- **AvgQuantityPerInvoice**  
- **AvgPurchaseAmount**

Additional analyses include:

- Revenue by country  
- Unique customers by country  
- Monthly sales trends  
- Top 10 customers by spending, quantity, and number of invoices  
- Distribution of spending and quantities  

---

## Visualizations
Visualizations were created using Matplotlib and Seaborn, including:

- Top 10 customers by spending  
- Top 10 customers by quantity  
- Revenue by country  
- Monthly revenue trends  
- Distribution of customer spending  
- Distribution of quantities per invoice  

---

## Key Insights
- The United Kingdom is the largest and most profitable market  
- Some countries show high revenue despite having fewer customers (e.g., Netherlands)  
- Sales peak in October–November, indicating seasonal demand  
- Customers exhibit highly diverse purchasing behavior  

---

## Business Recommendations
- Offer loyalty incentives to high-spending customers  
- Strengthen marketing efforts in the UK, Germany, and the Netherlands  
- Align promotions with seasonal sales peaks  
- Create product bundles for large-quantity purchasers  
- Identify and retain high-value, returning customers  

---

## Technologies Used
- **Python:** Pandas, Matplotlib, Seaborn  
- **Google Colab (Jupyter Notebook environment)**  
- **Data Source:** Kaggle Online Retail Dataset  

---

## Included Files
- `OnlineRetailAnalysis.ipynb` – full data analysis notebook
