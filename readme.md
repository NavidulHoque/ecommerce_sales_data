# E-Commerce Sales & Customer Analytics

A business analytics project based on 1,956 sales transactions from 287 customers across all 8 divisions of Bangladesh, covering January 2023 to December 2024.

The analysis was mainly built in Excel with additional data checking in Python and a Power BI version in progress. The goal is to turn sales data into simple business insights that sales and marketing teams can use.

---

## What This Project Does

The project answers two practical business questions:

1. **Why did total revenue fall in 2024, and where did the decline happen?**
2. **Which customers need the most attention to protect future revenue?**

It also helps answer questions such as:

- Which products and divisions generate the most revenue?
- How does revenue change from month to month and quarter to quarter?
- Which divisions are growing and which are declining?
- Who are the best customers?
- Which customers have stopped buying?
- Where should customer retention campaigns start?

### Key Findings

* Total revenue dropped by **4.21%**, from **BDT 162.47M in 2023 to BDT 155.62M in 2024**.
* The drop was **not a general slowdown**. Smartphones (**+1.14%**), Accessories (**+13.51%**), and Wearables (**+34.27%**) grew, but the two high-value products fell sharply: **Laptops (-10.77%)** and **Monitors (-13.90%)**.
* The problem started in the second half of 2024. Laptop sales were up in Q1 and Q2, then fell **19.27% in Q3** and **34.11% in Q4**.
* The damage was concentrated in specific divisions: **Chattogram** (Laptops -35.07%, Monitors -62.10%) and **Rangpur** (Laptops -83.72%). Dhaka, Rajshahi and Sylhet were still growing in Laptops.
* **43.21%** of customers (124 out of 287) are in "vulnerable" groups: At Risk, Lost/Churned or Low Engagement.
* The biggest single threat is the **78 At Risk customers**. They have a high average spend of **BDT 1.24M** each, but haven't bought anything for about **189 days** on average.
* **Dhaka (44.55%)** and **Chattogram (43.10%)** have the most vulnerable customers.

---

## Visualizations

### Excel: Detailed Business Analysis

The Excel workbook is the main part of this project. It contains two interactive dashboards, each focused on one of the main business questions.

The dashboards can be filtered using clickable filters, allowing users to view results for a specific division, product or customer group without needing technical knowledge.

#### 1. Sales Dashboard

Shows the overall sales performance of the business.

**Key figures:** 
- Total Revenue
- Total Orders
- Average Revenue per Order
- Total Quantity Sold

| View | What It Shows |
| ---- | ------------- |
| Revenue by Month | How revenue changes over time and when major increases or declines happened |
| Revenue by Division | Which divisions generate the most revenue |
| Revenue by Product Category | How Electronics, Accessories, and Wearables perform |
| Revenue by Products | Which products contribute the most revenue |
| Total Quantity (by month and by division) | How many units were sold over time and across divisions |

**Filters:** Gender, Division, Sales Channel, Product, Category and Date.

#### 2. Customer Segment Dashboard

Shows the different customer segments and how active and valuable they are.

The dashboard uses RFM analysis, which is simply a way to understand customer buying behavior.

> **What is RFM?**
> * **Recency**: How recently did the customer buy?
> * **Frequency**: How often does the customer buy?
> * **Monetary**: How much has the customer spent?
>
> Each customer receives a score from 1 to 5 for each measure. These scores are then used to place customers into seven groups.

**Key figures:** 
- Total Customers
- Total Revenue
- Total Transactions
- Average Customer Value
- Average Frequency
- Average Recency

| View | What It Shows |
| ---- | ------------- |
| Customer Count by Segment | How many customers are in each group |
| Revenue by Segment | How much revenue each group generates |
| Average Spending / Frequency / Recency by Segment | How much customers spend, how often they buy, and how recently they purchased |
| Frequency vs Monetary Value | Whether frequent buyers also tend to spend more |
| Frequency vs Recency | Which frequent buyers have stopped purchasing recently |
| Customer Type | The percentage of customers who are Active or Inactive |
| Customer Segment Distribution | The percentage of customers in each of the 7 customer segments |

**Filters:** Division, Customer Segment and Customer Type.

#### Excel Dashboard Screenshots

<!-- Add your dashboard screenshots to an /images folder and keep the file names below, or update the paths -->

![Excel Sales Dashboard](/images/sales-dashboard.png)

![Excel Customer Segment Dashboard](/images/customer-segment-dashboard.png)

#### Detailed Analysis Report

The Excel analysis was used to create a business report comparing 2023 and 2024, including the main findings and recommended actions.

**[Detailed Analysis Report](https://drive.google.com/file/d/1tgbJTymTYKr5M9bt8z35vYAOsCXgQi2d/view?usp=sharing)**

The full workbook, including every PivotTable, formula and chart, is available at:

`sales_data.xlsx`

### Power BI: Interactive Dashboard

An interactive Power BI dashboard is **coming soon**.

It will provide another interactive way to explore the same sales and customer findings. The project file (`ecommerce_sales_data.pbix`) already contains the sales and customer data and is ready for dashboard development.

---

## Dataset

The analysis uses **1,956 sales transactions** from **287 unique customers** between January 2023 and December 2024.

| Column | Description |
| ------ | ----------- |
| `Customer ID` | Unique customer identifier |
| `Gender` | Gender of the customer |
| `Division` | One of 8 divisions of Bangladesh |
| `Age` | Age of the customer |
| `Product Name` | One of 7 products: Laptop, Smartphone, Monitor, Smartwatch, Headphones, Keyboard, Mouse |
| `Category` | Electronics / Accessories / Wearables |
| `Unit Price` | Price of one unit in Bangladeshi Taka (BDT) |
| `Quantity` | Number of units ordered |
| `Total Price` | Order value in BDT |
| `Order Date` | Date of the order, covering 2023–2024 |

Additional fields used in the analysis:

* **Week Day and Day Type**: The day of the week, and whether it falls on a Weekday or Weekend.
* **Recency, Frequency and Monetary**: Shows how recently a customer purchased, how often they purchased, and how much they spent.
* **R, F and M Scores**: Scores from 1–5 for Recency, Frequency, and Monetary value.
* **Customer Segment**: The customer's RFM group, such as Champions, Loyal Customers, At Risk, or Lost/Churned.
* **Customer Type:** Shows whether the customer is currently Active or Inactive based on their customer segment.

---

## Analysis Covered

* Total revenue, orders, and units sold
* Revenue by month, quarter, and year
* Year-over-year revenue comparison
* Revenue by division, product, category
* Quantity sold over time and by division
* Laptop and Monitor sales decline by division and time
* Customer scoring and segmentation
* Customer count, spending, frequency, and recency by segment
* Relationship between frequency, spending, and recency
* Customer segment distribution across all 8 divisions

---

## Project Structure

| File / Folder | Purpose |
| ------------- | ------- |
| `sales_data.xlsx` | Main analysis workbook with the data, formulas, PivotTables, charts, slicers and both dashboards |
| `ecommerce_sales_data.pbix` | Power BI project file (dashboard coming soon) |
| `data/sales_data(cleaned data).csv` | Final sales dataset used for the analysis |
| `data/sales_data(raw data).csv` | Starting dataset used as the base of the project |
| `data_profiling.ipynb` | Python notebook used to check and profile the dataset |
| `data_profile_report.html` | Interactive data report that can be opened in a web browser |

**Inside `sales_data.xlsx`:**

| Sheet | Purpose |
| ----- | ------- |
| `Sales Dashboard` | Interactive sales dashboard |
| `Customer Segment Dashboard` | Interactive customer segmentation dashboard |
| `Sales Pivot Table` | Data summaries used for the Sales Dashboard |
| `Customer Segment Pivot Table` | Data summaries used for the Customer Segment Dashboard |
| `Customer RFM Table` | Customer RFM scores and segments |
| `Cleaned_Data` | Cleaned transaction data |
| `Raw_Backup` | Backup of the original data |

The Excel and Power BI files can be opened independently.

---

## Tech Stack

* **Excel**: Data analysis, PivotTables, filters, charts, dashboards, and customer segmentation
* **Power BI**: Interactive dashboard development
* **Python**: Data checking and automated data profiling

---

## About

Built by Navidul Hoque, a Backend Software Engineer transitioning into Data Science and AI.

This is one of my hands-on data analytics projects while pursuing a Post Graduate Diploma in Data Science with Machine Learning and Artificial Intelligence.

The project reflects my interest in using data, technology, and analytical thinking to understand real business problems and turn data into useful decisions.

Feedback and suggestions are welcome.

[LinkedIn](https://www.linkedin.com/in/navidul-hoque-04b850267)
