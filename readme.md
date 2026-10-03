# E-Commerce Sales & Customer Analytics

A business analytics project based on **1,956 sales transactions from 287 customers across all 8 divisions of Bangladesh**, covering **January 2023 to December 2024**. The project looks at where sales are growing, where they are shrinking, and which customers the business is at risk of losing.

The analysis was built in **Excel**, with a supporting data profiling report in **Python** and a **Power BI** version in progress. The goal is simple: turn raw sales records into clear answers that a sales or marketing team can act on.

---

## What This Project Does

The project answers two practical business questions:

1. **Why did total revenue fall in 2024, and where exactly did it fall?**
2. **Which customers should the business focus on first to protect its revenue?**

Along the way, the dashboards also help answer everyday questions such as:

* Which products, divisions and sales channels bring in the most revenue?
* How does revenue move month by month and quarter by quarter?
* Which regions are growing and which are slipping?
* Who are our best customers, and who has quietly stopped buying?
* Where should a retention or win-back campaign be aimed first?

### Key Findings

* **Total revenue dropped by 4.21%**, from **BDT 162.47M in 2023 to BDT 155.62M in 2024**.
* The drop was **not a general slowdown**. Smartwatches (**+34.27%**) and Headphones (**+20.65%**) grew, but the two high-value products fell sharply: **Laptops (-10.77%)** and **Monitors (-13.90%)**, together losing **BDT 11.51M**.
* The problem started in the **second half of 2024**. Laptop sales were up in Q1 and Q2, then fell **19.27% in Q3** and **34.11% in Q4**.
* The damage was **concentrated in specific divisions**: **Chattogram** (Laptops -35.07%, Monitors -62.10%) and **Rangpur** (Laptops -83.72%). Dhaka, Rajshahi and Sylhet were still growing in Laptops.
* **43.21% of customers (124 out of 287)** are in "vulnerable" groups: At Risk, Lost/Churned or Low Engagement.
* The biggest single threat is the **78 "At Risk" customers**. They have a high average spend of **BDT 1.24M** each, but haven't bought anything for about **189 days** on average.
* **Dhaka (44.55%)** and **Chattogram (43.10%)** have the most vulnerable customers, so the same two divisions face both the sales decline and the customer-loss risk.

---

## Visualizations

### Excel: Detailed Business Analysis

The Excel workbook is the heart of this project. It contains **two interactive dashboards**, each built to answer one of the business questions above. Both can be filtered with clickable buttons (slicers), so a manager can narrow the view to a single division, product, channel or customer group without any technical knowledge.

#### 1. Sales Dashboard

Shows how the business is performing in terms of revenue, orders and units sold.

**Key figures:** Total Revenue, Total Orders, Average Revenue per Order, Total Quantity Sold

| View | What It Shows |
| ---- | ------------- |
| Revenue by Month | How revenue rises and falls over time, making seasonal patterns and the late-2024 slump easy to spot |
| Revenue by Division | Which divisions drive the business (Dhaka and Chattogram together bring in roughly 58% of revenue) |
| Revenue by Product Category | Electronics, Accessories and Wearables compared |
| Revenue by Sales Channel | How revenue splits across Online, Retail Store, Marketplace and Corporate Sales |
| Top 3 Products by Revenue | The products the business depends on most (Laptops alone are about half of all revenue) |
| Total Quantity (by month and by division) | Units sold over time and by region, to tell apart "fewer units sold" from "lower-priced items sold" |

**Filters:** Gender, Division, Sales Channel, Product, Category, and a date timeline (Year / Quarter / Month / Day).

#### 2. Customer Segment Dashboard

Shows who the customers are and how valuable and active each group is, using **RFM segmentation**.

> **What is RFM?** It is a simple, widely used way to group customers by their buying behavior:
> * **Recency**: how recently did they last buy?
> * **Frequency**: how often do they buy?
> * **Monetary**: how much have they spent in total?
>
> Each customer is scored from 1 to 5 on each of the three measures, and the combination places them into one of seven easy-to-understand groups.

**Key figures:** Total Customers, Total Revenue, Total Transactions, Average Customer Value, Average Purchase Frequency, Average Recency

| View | What It Shows |
| ---- | ------------- |
| Customer Count by Segment | How many customers sit in each group |
| Revenue by Segment | How much money each group has brought in |
| Average Spending / Frequency / Recency by Segment | The "personality" of each group: big spenders, frequent buyers, or customers who have gone quiet |
| Frequency vs Monetary Value | Whether customers who buy often also spend more |
| Frequency vs Recency | Which frequent buyers have recently stopped coming back |

**Filters:** Division and Customer Segment.

#### Excel Dashboard Screenshots

<!-- Add your dashboard screenshots to an /images folder and keep the file names below, or update the paths -->

![Excel Sales Dashboard](/images/sales-dashboard.png)

![Excel Customer Segment Dashboard](/images/customer-segment-dashboard.png)

#### Detailed Analysis Report

The Excel analysis was used to produce a separate business report comparing **2023 and 2024**, with findings, business implications and recommended actions.

**[Detailed Analysis Report](ADD-YOUR-GOOGLE-DRIVE-LINK-HERE)**

The full workbook, including every PivotTable, formula and chart, is available at:

`sales_data.xlsx`

---

### Power BI: Interactive Dashboard

An interactive Power BI dashboard is **coming soon**.

The Power BI version will let users explore the same sales and customer segmentation findings in an interactive web-style report. The project file (`ecommerce_sales_data.pbix`) already contains the sales and customer segmentation data and is ready for dashboard design.

---

## Business Problem 1: Why Did High-Value Product Sales Fall?

**The situation:** Total revenue fell 4.21% even though unit sales of cheaper products were growing. The cause was hidden inside two expensive product lines.

**What the Sales Dashboard revealed:**

| Product | 2023 Revenue | 2024 Revenue | Change |
| ------- | -----------: | -----------: | -----: |
| Laptop | BDT 83.95M | BDT 74.91M | **-10.77%** |
| Monitor | BDT 17.79M | BDT 15.31M | **-13.90%** |
| Smartphone | BDT 43.30M | BDT 43.79M | +1.14% |
| Smartwatch | BDT 8.76M | BDT 11.76M | +34.27% |
| Headphones | BDT 4.53M | BDT 5.46M | +20.65% |

Growth in small, affordable items could not make up for the loss in Laptops and Monitors, because Laptops alone make up about half of all revenue.

**When it happened:** Laptop sales were healthy in the first half of 2024 (Q1 +7.61%, Q2 +7.20%), then fell in Q3 (-19.27%) and Q4 (-34.11%). In November 2024, Laptop revenue was only BDT 3.32M compared with BDT 9.23M in November 2023.

**Where it happened:**

| Division | Laptop Sales Change | Monitor Sales Change |
| -------- | ------------------: | -------------------: |
| Chattogram | **-35.07%** | **-62.10%** |
| Rangpur | **-83.72%** | +77.27% |
| Khulna | -25.00% | -4.76% |
| Dhaka | +16.43% | -8.07% |
| Rajshahi | +33.33% | -4.92% |
| Sylhet | +57.14% | +70.83% |

**What the business can do about it:**

1. **Investigate Chattogram and Rangpur first.** Review local channel partners, delivery costs and promotions in these two divisions to recover lost market share.
2. **Plan for the second half of the year.** Launch seasonal and corporate upgrade bundles (for example, Laptop + Monitor + Accessory with zero-cost EMI) from early Q3, before the slump begins.
3. **Win back past laptop buyers.** Reach out to customers who haven't made a high-value purchase in 12+ months with personal upgrade offers.
4. **Learn from the winners.** Dhaka, Rajshahi and Sylhet grew in Laptops, so what they are doing differently is worth studying.

---

## Business Problem 2: Which Customers Should We Focus On First?

**The situation:** The business has 287 customers, and a large share of them have gone quiet. Without a clear priority, retention budgets get spread too thin.

**What the Customer Segment Dashboard revealed:**

| Segment | Customers | Avg. Days Since Last Purchase | Avg. Orders | Avg. Total Spend |
| ------- | --------: | ----------------------------: | ----------: | ---------------: |
| Champions | 50 | 21 | 9.24 | BDT 1,857,817 |
| At Risk | 78 | 189 | 6.72 | BDT 1,235,220 |
| Loyal Customers | 58 | 45 | 8.76 | BDT 1,063,335 |
| Potential Loyal | 34 | 53 | 5.59 | BDT 1,005,887 |
| New Customers | 21 | 23 | 4.57 | BDT 779,293 |
| Lost / Churned | 37 | 242 | 3.73 | BDT 379,605 |
| Low Engagement | 9 | 67 | 4.22 | BDT 284,677 |

**In plain English:**

* **Champions and Loyal Customers (108 customers)** are the core of the business: they buy often, spend a lot and bought recently.
* **At Risk customers (78)** are the most important finding. They used to buy frequently and spend heavily, but have been silent for over six months. They are worth far more than the Lost/Churned group, so they are the best place to put retention effort.
* **Potential Loyal and New customers (55)** are the growth pipeline, recent buyers who could become loyal with the right nudge.
* **Lost/Churned and Low Engagement customers (46)** spent little and have been gone the longest, so they are not worth costly campaigns.

**Where the risk is concentrated:**

| Division | Vulnerable Customers | Share of Division's Customers |
| -------- | -------------------: | ----------------------------: |
| Dhaka | 45 of 101 | 44.55% |
| Chattogram | 25 of 58 | 43.10% |
| Rajshahi | 13 of 29 | 44.83% |
| Khulna | 12 of 30 | 40.00% |

Customer loss is not a problem of one region. It affects every major division.

**Recommended action plan, in priority order:**

| Priority | Who | Focus Divisions | Recommended Action |
| :------: | --- | --------------- | ------------------ |
| 1 | **At Risk** customers | Dhaka (27), Chattogram (19) | Automated win-back campaigns with exclusive loyalty discounts on Laptops and Monitors |
| 2 | **Champions and Loyal** customers | Dhaka (35), Chattogram (21) | Dedicated account support, early access to new products and bulk-purchase perks |
| 3 | **Potential Loyal and New** customers | Dhaka (21), Chattogram (12) | Cross-selling onboarding, such as recommending monitors and accessories to recent laptop buyers |
| 4 | **Lost/Churned and Low Engagement** customers | All divisions | Low-cost automated emails during major clearance events, with no expensive targeted campaigns |

---

## How the Two Problems Connect

The two analyses point to the same places. **Chattogram** has both the sharpest drop in high-value sales and a large group of at-risk customers, and **Dhaka** has the largest number of customers at risk. A win-back campaign built around **Laptops and Monitors** in **Dhaka and Chattogram** addresses both problems at once.

---

## Dataset

The analysis uses **1,956 sales transactions** from **287 unique customers** between January 2023 and December 2024.

| Column | Description |
| ------ | ----------- |
| `Order ID` | Unique order number |
| `Customer ID` | Unique customer identifier |
| `Gender` | Gender of the customer |
| `Division` | One of 8 divisions of Bangladesh |
| `Age` | Age of the customer |
| `Sales Channel` | Online / Retail Store / Marketplace / Corporate Sales |
| `Product Name` | One of 7 products: Laptop, Smartphone, Monitor, Smartwatch, Headphones, Keyboard, Mouse |
| `Category` | Electronics / Accessories / Wearables |
| `Unit Price` | Price of one unit in Bangladeshi Taka (BDT) |
| `Quantity` | Number of units ordered |
| `Total Price` | Order value in BDT |
| `Order Date` | Date of the order, covering 2023–2024 |

Additional fields used in the analysis:

* **Week Day and Day Type**: the day of the week, and whether it falls on a Weekday or Weekend (Friday and Saturday, the weekend in Bangladesh)
* **Year, Quarter and Month**: used for trend and year-over-year comparisons
* **Recency, Frequency and Monetary**: each customer's days since last purchase, number of orders and total spend
* **R, F and M Scores**: each customer's 1–5 score on the three measures above
* **Customer Segment**: one of the 7 RFM groups (Champions, Loyal Customers, Potential Loyal, New Customers, At Risk, Lost/Churned, Low Engagement)

---

## Analysis Covered

* Total revenue, orders and units sold
* Revenue by month, quarter and year, with year-over-year comparison
* Revenue by division, product, product category and sales channel
* Top products by revenue
* Quantity sold over time and by division
* Divisional and quarterly breakdown of the Laptop and Monitor decline
* RFM scoring and customer segmentation
* Customer count, revenue, spending, frequency and recency by segment
* Relationship between purchase frequency, spending and recency
* Segment distribution across all 8 divisions

---

## Project Structure

| File / Folder | Purpose |
| ------------- | ------- |
| `sales_data.xlsx` | Main analysis workbook with the data, formulas, PivotTables, charts, slicers and both dashboards |
| `ecommerce_sales_data.pbix` | Power BI project file (dashboard coming soon) |
| `data/sales_data(cleaned data).csv` | Final sales dataset used for the analysis |
| `data/customer_segmentation.csv` | Customer-level RFM results and segments |
| `data/sales_data(raw data).csv` | Starting dataset used as the base of the project |
| `data_profiling.ipynb` | Python notebook that automatically profiles the dataset |
| `data_profile_report.html` | Interactive profiling report. Open it in any web browser |

**Inside `sales_data.xlsx`:**

| Sheet | Purpose |
| ----- | ------- |
| `Sales Dashboard` | Interactive sales performance dashboard |
| `Customer Segment Dashboard` | Interactive customer segmentation dashboard |
| `Sales Pivot Table` | PivotTables that power the Sales Dashboard |
| `Customer Segment Pivot Table` | PivotTables that power the Customer Segment Dashboard |
| `Customer RFM Table` | Each customer's RFM scores and segment, calculated with Excel formulas |
| `Cleaned_Data` | The full transaction dataset |
| `Raw_Backup` | Backup of the starting data |

The Excel and Power BI files can be opened independently. The profiling report (`data_profile_report.html`) opens in any browser with no setup.

---

## Tech Stack

* **Excel**: PivotTables, slicers, timeline filter, charts, dashboards, and formulas (`XLOOKUP`, `PERCENTILE.INC`, nested `IF` logic) for RFM scoring and segmentation
* **Power BI**: interactive dashboard (in progress)
* **Python (Pandas, ydata-profiling)**: automated data profiling report

---

## About

Built by **Navidul Hoque**, a Backend Software Engineer transitioned into Data Science and AI.

This is one of my first hands-on data analytics projects while pursuing a **Post Graduate Diploma in Data Science with Machine Learning and Artificial Intelligence**.

The project reflects my interest in using **data, technology, and analytical thinking to understand real-world business problems** and turn them into decisions a team can act on.

Feedback and suggestions are welcome.

[LinkedIn](https://www.linkedin.com/in/navidul-hoque-04b850267)
