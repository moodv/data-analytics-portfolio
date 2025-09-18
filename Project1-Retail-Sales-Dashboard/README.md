# Project 1 — Retail Sales Dashboard (RFM Analysis & Insights)

**Author:** Mahmoud Elnaggar 
**Tools:** Python (pandas, matplotlib/seaborn), Google Colab Notebook, Power BI.  
**Dataset:** Kaggle — Supermarket Sales (download CSV and place in `data/`)

## Summary
End-to-end analysis of retail sales: cleaning, EDA,  and a dashboard highlighting business insights and retention recommendations.

📌 Project Overview

This project demonstrates my ability to perform data cleaning, exploratory data analysis (EDA), and dashboard creation using a retail sales dataset.
The dataset includes 1,000 sales records × 17 columns over the first three months of the year.
Since the dataset is relatively small, this project is intended as a demonstration of analytical skills, not as a production-level case study.

⚙️ Tools & Technologies

* Python (Pandas, Matplotlib, Seaborn) → Data cleaning & preprocessing
* Power BI → Interactive dashboards & visualizations
* Git/GitHub → Version control & project management

🔑 Key Steps

**1. Data Cleaning (Python)**
   * Removed duplicates & missing values
   * Normalized categorical fields (branch names, cities, product lines)
   * Converted date/time columns into day & month
   * Created calculated fields (e.g., revenue, profit margin)

**2. Exploratory Analysis (Python & Power BI)**
   * Sales & profit by branch
   *  Performance across product lines
   *  Impact of customer type (Member vs Normal)
   *  Payment preferences (Cash, Credit Card, E-wallet)
   *  Trends by day of week and time of day

3. Dashboard Development (Power BI)
   * Branch & Product Line Analysis
   * Customer Type & Payment Analysis
   * Time Trends (Daily/Weekly/Monthly)


📊 Key Insights

1. **Branches** performed differently: Branch C generated the highest revenue, while Branch A had the strongest performance in certain product lines.
2. **Product Lines**: Food & Beverages and Sports & Travel had the highest overall revenue, while Health & Beauty showed lower but steady sales.
3. **Customer Types**: Members contributed significantly more revenue than normal customers, confirming the value of loyalty programs.
4. **Payment Methods** were evenly distributed across Cash, Credit Card, and E-wallet, with no single dominant method — suggesting customers value multiple payment options.
5. **Time Trends**:
   * Weekends (especially Saturday) saw the highest sales volume and revenue.
   * Afternoon was the most profitable time of day, followed by evenings.

📊 Dashboard Preview

(dashboard or .pbix file here `dashboard/`)

⚠️ Note on Customer Segmentation:
The dataset did not include a true customer_id column, only invoice_id.
Because of this, advanced customer-level analysis (like RFM segmentation) was not possible in this project.
Future projects will use larger datasets with proper customer identifiers to explore customer segmentation, churn, and clustering.

## Contact
Mahmoud Elnaggar  — mahmoud.elnaggar19@gmail.com

