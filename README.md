---

# **Customer Analysis Project – Online Retail**

## **Project Description**

This project analyzes customer purchases from an online retail store with the goal of understanding **customer behavior**, **key metrics**, and generating business insights.
The dataset includes information on purchases, products, quantities, prices, invoices, and countries.

---

## **Project Steps**

### **Step 1 – Load Data**

* Upload a CSV file containing all purchases.
* Initial inspection of missing data, column types, and number of rows.

### **Step 2 – Data Cleaning**

* Remove rows with missing `CustomerID` or `Description`.
* Remove rows with `Quantity` or `UnitPrice` less than or equal to 0.
* Convert `InvoiceDate` to datetime format.
* Create `Year` and `Month` columns.

### **Step 3 – Calculate Metrics**

Key metrics per customer:

| Metric                 | Description                                           |
| ---------------------- | ----------------------------------------------------- |
| TotalPrice             | Total money spent per purchase (Quantity * UnitPrice) |
| TotalSpent             | Total spending per customer (sum of TotalPrice)       |
| TotalQuantity          | Total number of products purchased by the customer    |
| NumInvoices            | Number of unique invoices per customer                |
| AvgQuantityPerInvoice  | Average quantity of products per invoice              |
| AvgProductsPerPurchase | Average quantity of products per purchase             |
| AvgPurchase            | Average purchase amount per customer                  |

Metrics by country:

| Metric                   | Description                            |
| ------------------------ | -------------------------------------- |
| TotalSpentByCountry      | Total revenue per country              |
| UniqueCustomersByCountry | Number of unique customers per country |

Metrics over time:

| Metric                | Description                        |
| --------------------- | ---------------------------------- |
| PurchasePerMonth      | Total purchases per month          |
| MonthlyAndYearlySales | Total purchases per month and year |

---

### **Step 4 – Customer Profile**

* A `CustomerProfile` DataFrame was created with all metrics for each customer.
* Enables comparison between customers based on purchases, product quantities, and averages.

---

### **Step 5 – Graphs & Dashboards**

| Graph                                         | Description                                                                         |
| --------------------------------------------- | ----------------------------------------------------------------------------------- |
| Top 10 Customers by Total Purchases           | Shows the top 10 customers who spent the most in total.                             |
| Top 10 Customers by Total Quantity            | Shows the top 10 customers who purchased the most products overall.                 |
| Top 10 Customers by Number of Invoices        | Shows the top 10 customers with the highest number of unique invoices.              |
| Top 10 Countries by Unique Customers          | Shows the 10 countries with the highest number of unique customers.                 |
| Monthly Sales by Year                         | Displays total purchases per month, separated by year, to identify seasonal trends. |
| Number of Purchases per Month                 | Shows the number of purchases (invoices) for each month.                            |
| Top 10 Countries by Revenue                   | Shows the top 10 countries generating the most revenue.                             |
| Distribution of Total Purchases per Customer  | Histogram showing the distribution of total purchases across customers.             |
| Distribution of Average Quantity per Customer | Histogram showing the distribution of average products per customer.                |

*All graphs are in English, with Hebrew comments in the code for explanation.*

---

### **Insights**

1. Some customers spend very high amounts, although their number of purchases may be low (premium customers).
2. The UK generates the highest revenue and has the largest number of customers.
3. Other countries like the Netherlands generate significant revenue but are not in the top 10 by number of customers, and Germany, which has the second-highest number of customers, ranks fourth in revenue.
4. Certain months (October and November) show higher sales, while December appears high because it was recorded twice. Most other months only have data from one year.
5. Customers vary in their purchase behavior: some buy fewer invoices but many products (e.g., Customer 14606, who also spent the most), while others buy many invoices but fewer products (e.g., Customer 12748), and these are not in the top 10 by total items or spending.

---

### **Business Recommendations**

1. **High-spending customers:** Offer tailored promotions or loyalty programs.
2. **Leading countries:** Invest in marketing and faster delivery in these regions (UK, Germany, Netherlands).
3. **Seasonal trends:** Align promotional campaigns with high-sales months (October and November).
4. **Customer behavior analysis:** Identify which products are purchased by high-average customers and consider bundles or upsell opportunities.
5. **Customer retention:** Analyze average purchase amounts and product quantities to identify high-potential returning customers.

---

### **Tools & Technologies**

* Python (Pandas, Matplotlib, Seaborn)
* Google Colab

---

### **Project Files**

* `OnlineRetail.csv` – Raw dataset
* Python code for data cleaning, analysis, and graph creation

---

רוצה שאעשה זאת?
