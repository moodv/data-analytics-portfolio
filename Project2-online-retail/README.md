# project2: online retail customer segmentation

📊 Customer Insights Dashboard – Project 2
🔹 Project Overview

DATASETS: You can find all datasets used in this project from;
The Original Dataset:  https://archive.ics.uci.edu/dataset/352/online+retail .
All Pre-Processed Datasets: https://drive.google.com/file/d/1qRtuTBz86wFV_7k1eBZlmCErYeAbDHfh/view?usp=sharing .

This project is an end-to-end data analytics and business intelligence solution. It covers everything from data engineering & preprocessing in Google Colab to building a multi-page interactive dashboard in Power BI.

The goal was to uncover customer behavior, profitability, and growth opportunities by analyzing customer transactions, journeys, and segmentation.

🔹 Tools & Technologies

* Google Colab (Python) → Data preprocessing, cleaning, transformations.
* Pandas / NumPy → Data wrangling & feature engineering.
* Matplotlib / Seaborn → Quick exploratory analysis & validation.
* Power BI → Data modeling, DAX measures, dashboards.
* DAX (Data Analysis Expressions) → KPIs, RFM segmentation, profitability, and lifetime metrics.
* GitHub → Repository for version control, documentation, and notebook sharing.

🔹 Data Engineering (in Google Colab)
The raw data was processed and cleaned in Python before importing into Power BI. Steps included:

* Data Cleaning → Removed nulls, duplicates, inconsistent data types.

* Feature Engineering →
1. Created Recency, Frequency, Monetary (RFM) variables.
2. Computed first/last purchase dates for customers.
3. Calculated returns and profit fields.

* Data Validation → Basic stats & visual checks to ensure consistency.
* Export → Final datasets exported as CSV files → used as inputs for Power BI.
* Notebook: EDA.ipynb (included in this repo).

🔹 Data Sources

* Customers dataset → RFM scores, segmentation, customer-level features.
* Customer Journey dataset → First purchase, last purchase, recency tracking.
* Transactions dataset → Sales, quantity, returns, cost, revenue, profit.
* Segment Summary dataset → Pre-computed segment breakdown for validation.

🔹 Dashboard Pages & Insights
1️⃣ Page 1: Executive Overview: 

* KPIs: Total Sales, Profit, Returns.
* Top Products & Return Analysis.
* High-level customer and product health.

2️⃣ Page 2: Customer Insights – RFM Segmentation:

* RFM buckets (Recency, Frequency, Monetary).
* Segment distribution: Champions, At Risk, Lost, etc.
* Customer behavioral patterns.
* Active, New, and Churned customers.
* 
3️⃣ Page 3: Customer Journey & Lifetime

* Customer Life Value
* Active vs Churned customers by year.
* Average Customer Lifetime.
* Retention Rate over month

4️⃣ Page 4: Customer Profitability & Growth Drivers

* Top 5 customers by profit.
* Profit distribution histogram.
* Profit Margin % by Segment.


🔹 Key Features

* End-to-End Workflow: Data engineering in Python + BI dashboard in Power BI.
* Structured Approach: Each dashboard page answers a different business question (no duplication).
* Action-Oriented: Helps management identify profitable customers, at-risk segments, and key growth opportunities.
* Scalable: Easy to add predictive analytics (e.g., churn prediction, sales forecasting).



🔹 Future Improvements

Automate pipeline: Colab → Power BI Service refresh.

Integrate marketing spend to analyze ROI by segment.

Add predictive models (churn prediction, customer lifetime value forecasting).

✍️ Author: Mahmoud Elnaggar
🎯 Role: Data Analyst (Portfolio Project)
