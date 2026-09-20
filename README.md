# 📊 Sales Insight Dashboard

An interactive **Customer Insights & Sales Analytics Dashboard** built using **SQL, Python (Pandas), and Power BI** to analyze sales performance, customer behavior, purchasing patterns, and customer engagement.

The project transforms raw customer transaction data into actionable business insights through **data cleaning, SQL analysis, KPI development, DAX measures, and interactive Power BI visualizations**.

---

## 🎯 Business Problem

Businesses generate large volumes of customer and sales data, but raw data alone does not provide an easy way to understand business performance.

This project focuses on answering key business questions:

* How much revenue is being generated?
* Which customer segments contribute the most to sales?
* Which product categories perform best?
* What are the purchasing patterns of customers?
* How engaged are customers with subscriptions?
* Which shipping and payment methods are preferred?
* How do discounts and promotions affect purchasing behavior?
* How satisfied are customers?

The dashboard brings these insights together into an interactive reporting solution for faster and more informed decision-making.

---

## 📌 Dashboard KPIs

| KPI                        |        Value |
| -------------------------- | -----------: |
| 👥 Total Customers         |    **3,900** |
| 💰 Total Sales             | **$233.08K** |
| 🛒 Average Purchase Value  |   **$59.76** |
| ⭐ Average Rating           | **3.75 / 5** |
| 🔄 Previous Purchases      |     **99K+** |
| 📈 Avg. Previous Purchases |    **25.35** |
| 👤 Male Sales Contribution |      **68%** |
| 🔔 Subscription Rate       |      **27%** |

---

## 🔍 Key Business Insights

### 🛍️ Product & Category Insights

* **Clothing** is the highest revenue-generating category.
* Accessories and Footwear are other major contributors to sales.
* Customer spending remains relatively consistent across product categories.

### 👥 Customer Insights

* Male customers contribute approximately **68% of total sales**.
* **Young Adults and Middle-aged customers** represent important spending segments.
* The dataset contains **3,900 customers**, allowing customer behavior to be analyzed across demographic groups.

### 🚚 Shipping & Payment Insights

* **Free Shipping** is the most preferred shipping option.
* Customer payment methods are relatively evenly distributed across the available payment options.
* Understanding payment and shipping preferences can help businesses optimize the customer experience.

### ⭐ Customer Satisfaction

* The average customer rating is **3.75 / 5**.
* This provides a useful indicator for monitoring customer satisfaction and product experience.

### 🔔 Subscription & Engagement

* Only **27% of customers are subscribers**.
* This indicates an opportunity to analyze customer engagement and develop strategies for increasing subscription adoption.

### 📅 Seasonal Trends

* Sales remain relatively consistent across the four seasons.
* This suggests that customer demand is distributed throughout the year rather than being concentrated in a single season.

---

## 🛠️ Tools & Technologies

### Data Analysis

* **Python**
* **Pandas**
* **Jupyter Notebook**

### Database & SQL

* **SQL**
* Data aggregation
* Filtering
* GROUP BY
* CASE statements
* Customer and sales analysis

### Business Intelligence

* **Microsoft Power BI**
* Power Query
* DAX
* Data Modeling
* Interactive Visualizations
* KPI Cards
* Slicers & Filters

---

## 🔄 Project Workflow

```text
Raw Customer Data
       ↓
Data Cleaning
       ↓
Python / Pandas
       ↓
SQL Analysis
       ↓
Data Modeling
       ↓
DAX Measures & KPIs
       ↓
Power BI Dashboard
       ↓
Business Insights
```

---

## 📊 Dashboard Pages

### 1️⃣ Executive Overview

Provides a high-level view of overall business performance.

![Executive Dashboard](Screenshots/excutive.png)

**Includes:**

* Total Sales
* Total Customers
* Average Purchase Value
* Average Rating
* Subscription Rate
* Sales by Gender
* Revenue by Category
* Revenue by Season
* Shipping Preferences
* Payment Preferences

### 2️⃣ Customer Insights

Provides a deeper analysis of customer behavior.

![Customer Insights Dashboard](Screenshots/customer.png)

**Includes:**

* Customer demographics
* Age-group analysis
* Purchase behavior
* Previous purchases
* Purchase frequency
* Subscription behavior
* Discount usage
* Shipping preferences
* Customer segmentation

---

## 📈 Key KPIs & DAX Measures

Examples of the measures developed for the dashboard include:

```DAX
Total Sales =
SUM(customers[purchase_amount])

Total Customers =
DISTINCTCOUNT(customers[customer_id])

Average Purchase Value =
AVERAGE(customers[purchase_amount])

Average Review Rating =
AVERAGE(customers[review_rating])

Subscription Rate =
DIVIDE(
    CALCULATE(
        DISTINCTCOUNT(customers[customer_id]),
        customers[subscription_status] = "Yes"
    ),
    [Total Customers]
)
```

---

## 💡 Business Value

The dashboard helps stakeholders:

* Monitor overall sales performance
* Identify high-performing product categories
* Understand customer demographics
* Analyze purchasing behavior
* Monitor customer satisfaction
* Evaluate subscription engagement
* Understand shipping and payment preferences
* Identify potential customer-growth opportunities

---

## 📂 Project Structure

```text
Sales-Insight/
│
├── 📁 Dataset/
│   └── shopping_trends.csv
│
├── 📁 Python/
│   └── sales_analysis.ipynb
│
├── 📁 SQL/
│   └── sales_analysis.sql
│
├── 📁 PowerBI/
│   └── Sales Insight Dashboard.pbix
│
├── 📁 Images/
│   ├── dashboard-overview.png
│   └── customer-insights.png
│
└── README.md
```

---

## 🎯 Skills Demonstrated

* Data Cleaning & Transformation
* Exploratory Data Analysis
* SQL Data Analysis
* Customer Segmentation
* KPI Development
* DAX
* Power BI Data Modeling
* Data Visualization
* Business Intelligence
* Business Insight Generation
* Dashboard Design

---

## 📌 Dataset

The project uses the **Customer Shopping Trends Dataset**, containing **3,900 customer records** covering demographics, purchases, product categories, ratings, subscriptions, shipping, payment methods, discounts, and purchasing frequency. The dataset is synthetic and intended for analytics/learning purposes.

---

## 👩‍💻 Author

**Shelly**

Data Analyst | SQL | Python | Power BI | Excel

🔗 GitHub: **keliya-shelly**
