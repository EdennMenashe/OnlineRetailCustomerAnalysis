---

# **Customer Analysis Project – Online Retail**

## **Project Description**

This project analyzes customer purchases from an online retail store to understand **customer behavior**, **key metrics**, and to generate actionable business insights.
The dataset includes information on purchases, products, quantity, price, invoices, and country.

---

## **Project Workflow**

### **Step 1 – Data Loading**

* Upload the CSV file containing all purchases.
* Perform initial checks for missing data, column types, and dataset size.

### **Step 2 – Data Cleaning**

* Remove rows with missing `CustomerID` or `Description`.
* Remove rows with negative or zero `Quantity` or `UnitPrice`.
* Convert the `InvoiceDate` column to datetime format.
* Create new columns for `Year` and `Month`.

### **Step 3 – Metrics Calculation**

Key metrics per customer:

| Metric                 | Description                                          |
| ---------------------- | ---------------------------------------------------- |
| TotalPrice             | Total money for each purchase (Quantity * UnitPrice) |
| TotalSpent             | Total spending per customer                          |
| TotalQuantity          | Total products purchased by the customer             |
| NumInvoices            | Number of unique invoices per customer               |
| AvgQuantityPerInvoice  | Average quantity per invoice for the customer        |
| AvgProductsPerPurchase | Average quantity of products per purchase (Invoice)  |
| AvgPurchase            | Average purchase amount per customer                 |

Metrics by country:

| Metric                   | Description                            |
| ------------------------ | -------------------------------------- |
| TotalSpentByCountry      | Total revenue per country              |
| UniqueCustomersByCountry | Number of unique customers per country |

Metrics by time:

| Metric                | Description                        |
| --------------------- | ---------------------------------- |
| PurchasePerMonth      | Total purchases per month          |
| MonthlyAndYearlySales | Total purchases per month and year |

---

### **Step 4 – Customer Profile**

* A `CustomerProfile` DataFrame is created with all metrics per customer.
* This allows comparing customers by total spending, product quantity, and averages.

---

### **Step 5 – Graphs and Dashboards**

The following visualizations were created:

1. Top 10 Customers by TotalPrice
2. Top 10 Customers by TotalQuantity
3. Top 10 Customers by NumInvoices
4. Top 10 Countries by Unique Customers
5. Monthly Sales by Year
6. Number of Purchases per Month
7. Top 10 Countries by Revenue
8. Distribution of Total Purchases per Customer (Histogram)
9. Distribution of Average Quantity per Customer (Histogram)

*All graphs are in English, with Hebrew comments in the code for explanations.*

---

### **Key Insights**

1. **High-spending customers:** Some customers spend a very high amount with few purchases (premium customers).
2. **Top countries:** The UK generates the highest revenue and has the most customers. Countries like Netherlands generate high revenue with fewer customers, and Germany has many customers but lower revenue. Marketing strategies can be adapted accordingly.
3. **Strong months:** October and November are the strongest months in sales, while other months are measured for only one year. December appears twice, so it seems higher but not necessarily accurate. These months may coincide with holiday seasons and are suitable for seasonal campaigns.
4. **Customer purchase patterns:** Some customers make fewer purchases but buy a large number of products per purchase (e.g., Customer 14606), leading to high spending. Other customers with many invoices (e.g., Customer 12748) purchase fewer items per invoice and are not in the top 10 by total items or spending.
5. **Diverse purchasing behavior:** Average quantity per purchase and average spending per customer indicate varied customer tendencies.

---

### **Business Recommendations**

1. **High-spending customers:** Offer personalized deals or loyalty programs.
2. **Top-performing countries:** Invest in marketing and fast shipping in high-revenue countries. Learn from Netherlands’ strategy for better targeting.
3. **Customers with few but large purchases:** Analyze customers who buy many products per purchase and provide bundles, upsell opportunities, or premium products.
4. **Customer retention:** Analyzing average purchases and product quantities helps identify high-potential repeat customers and optimize retention strategies.

---

### **Tools and Technologies**

* Python (Pandas, Matplotlib, Seaborn)
* Google Colab

---

### **Project Files**

* `OnlineRetail.csv` – raw dataset
* Python code for data cleaning, analysis, and graph generation

---


Do you want me to do that?
