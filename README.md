
---

# **Customer Analysis Project – Online Retail**

## **Project Description**

This project analyzes customer purchasing behavior in an online retail store (Online Retail) to understand **customer behavior**, **key metrics**, and generate actionable business insights.
The dataset includes information on purchases, products, quantities, prices, invoices, and countries.

---

## **Project Workflow**

### **Step 1 – Data Loading**

* Upload the CSV file containing all purchases.
* Perform an initial check for missing values, data types, and number of rows.

### **Step 2 – Data Cleaning**

* Remove rows with missing values in `CustomerID` or `Description`.
* Remove rows with negative or zero `Quantity` or `UnitPrice`.
* Convert the `InvoiceDate` column to datetime format.
* Create `Year` and `Month` columns for analysis.

### **Step 3 – Metrics Calculation**

Key metrics per customer:

| Metric                 | Description                                                  |
| ---------------------- | ------------------------------------------------------------ |
| TotalPrice             | Total money for each purchase (Quantity * UnitPrice)         |
| TotalSpent             | Total spending per customer (sum of TotalPrice per customer) |
| TotalQuantity          | Total number of products purchased by the customer           |
| NumInvoices            | Number of unique invoices per customer                       |
| AvgQuantityPerInvoice  | Average quantity of products per invoice                     |
| AvgProductsPerPurchase | Average number of products per purchase (Invoice)            |
| AvgPurchase            | Average purchase value per customer                          |

Country-level metrics:

| Metric                   | Description                            |
| ------------------------ | -------------------------------------- |
| TotalSpentByCountry      | Total revenue per country              |
| UniqueCustomersByCountry | Number of unique customers per country |

Time-based metrics:

| Metric                | Description                        |
| --------------------- | ---------------------------------- |
| PurchasePerMonth      | Total purchases per month          |
| MonthlyAndYearlySales | Total purchases per month and year |

---

### **Step 4 – Customer Profile**

* Create a `CustomerProfile` DataFrame with all metrics for each customer.
* Enables comparison of customers by spending, quantity, and averages.

---

### **Step 5 – Graphs and Dashboards**

1. Top 10 Customers by TotalPrice
2. Top 10 Customers by TotalQuantity
3. Top 10 Customers by NumInvoices
4. Top 10 Countries by Unique Customers
5. Monthly Sales by Year
6. Number of Purchases per Month
7. Top 10 Countries by Revenue
8. Distribution of Total Purchases per Customer (Histogram)
9. Distribution of Average Quantity per Customer (Histogram)

*All graphs are in English, with comments in Hebrew in the code for explanation.*

---

### **Preliminary Insights**

* Some customers spend very high amounts but may have few purchases (premium customers).
* Certain countries contribute the majority of revenue, so marketing focus there is important.
* Some months show higher sales, which can guide seasonal campaigns.
* Average quantity per purchase shows that some customers tend to buy more products per transaction.

---

### **Business Recommendations**

1. **High-spending customers:** Offer personalized promotions or loyalty programs.
2. **Top-revenue countries:** Invest in marketing and fast shipping in these regions.
3. **High-sales months:** Schedule seasonal campaigns based on peak purchasing months.
4. **Customers with high average purchase quantities:** Analyze the products they buy and offer bundles or upsell opportunities.
5. **Customer retention:** Analyze average purchases and quantities to identify potential repeat customers.

---

### **Tools and Technologies**

* Python (Pandas, Matplotlib, Seaborn)
* Google Colab

---

### **Project Files**

* `OnlineRetail.csv` – raw dataset
* Python code for data cleaning, analysis, and graph creation

---

