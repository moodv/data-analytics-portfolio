1. Introduction

This project presents a comprehensive HR Analytics and Employee Attrition Prediction system designed to uncover workforce trends, performance drivers, and potential attrition risks.
The goal was to move from raw HR data to actionable business insights through a complete data pipeline — encompassing database modeling, SQL exploration, predictive modeling in Python, and visualization in Power BI.
The outcome is an interactive analytics dashboard that empowers HR managers to understand employee behavior, training impact, and attrition risk with both descriptive and predictive insights.

2. Project Objectives

Analyze workforce demographics and performance patterns.
Measure training efficiency, ROI, and its impact on employee satisfaction.
Identify the key factors influencing employee attrition.
Predict which employees are at high risk of leaving the company using machine learning.

3. Tools and Technologies

The project integrates multiple technologies in a single analytical workflow:
Python: Data preprocessing, machine learning (Logistic Regression, Random Forest, XGBoost).
PostgreSQL (Neon Cloud): Data storage, SQL exploration, and creation of analytical views.
Power BI & DAX: Dashboard development and storytelling through visual analytics.
GitHub: Version control and project documentation.

4. Data Model Design

The data was modeled into a star schema for efficient analytics in Power BI.
It consists of four main dimension tables and one fact table.

Dimension Tables

dim_employee: Personal details such as age, gender, race, and state.
dim_employment: Department type, business unit, division, and tenure.
dim_training: Training type, cost, duration, and outcomes.
dim_performance: Performance scores, satisfaction, and engagement.
dim_date: Contains all time-based attributes for training, employment, and survey dates.

Fact Table

fact_employee_attrition: Central table linking all dimensions using employee_id.
It includes flags for attrition, satisfaction, engagement, and predictive outputs.

Relationships:
Each of the dimension tables has a many-to-one relationship with fact_employee_attrition, forming a clean star schema.

5. Methodology

The project followed a structured workflow:

5.1 Data Preparation

Data was imported into Neon PostgreSQL, normalized into lowercase column naming, and divided into the following tables:
employees, employment, performance, and training.
SQL queries were used to clean and transform data, calculate KPIs (such as engagement scores and tenure years), and prepare it for Power BI ingestion.

5.2 Machine Learning Model

Using Python, a predictive pipeline was built to estimate attrition probability.
Three algorithms were tested:
Logistic Regression – baseline model
Random Forest – best performing model (F1 Score: 0.87)
XGBoost – strong but slightly overfitted

The final Random Forest model was selected for its balanced performance and interpretability.
Predicted probabilities were exported as part of the fact table and visualized in Power BI.

6. Dashboard Design and Insights

The Power BI dashboard consists of four interactive pages, each serving a unique analytical purpose.

Page 1 – Workforce Demographics & Employment
This page provides an overview of employee demographics and hiring patterns.
Key metrics include:

Average Age: 49.45 years
Average Tenure: 5 years
Work-Life Balance: 2.99

Visuals:

Department hires by year
Age group distribution by department
Performance vs Work-Life Balance
Employee status trends
Employee type breakdown

Insight:
IT and Production departments exhibit the most hiring activity, with most employees aged 25–35.

Page 2 – Training & Performance Overview

This page explores how training affects performance, engagement, and ROI.
Key metrics include:

Total Trainings: 2,845
Average Training Days: 2.97
Training ROI: 0.53%

Visuals:

Engagement vs Satisfaction scatter
Training cost by department
Program completion vs failure rate
Outcome distribution and average ratings

Insight:
Production and IT departments demonstrate a strong link between training investment and improved performance outcomes.

Page 3 – Employee & Attrition Overview

This section focuses on analyzing attrition rates and identifying risk patterns.
Key metrics include:

Total Employees: 2,845
Attrited Employees: 387
Attrition Rate: 13.6%
Average Engagement Score: 2.94

Visuals:

Attrition by State, Division, Department Type, and Age Group
Demographic analysis by Race and Gender

Insight:
Attrition is most common among employees aged 25–35, primarily within IT and Production divisions.

Page 4 – Predictive Insights (Attrition Probability)

This page introduces the predictive layer powered by the Random Forest model.

Purpose:
To visualize and interpret model-driven attrition risk scores.

Visuals:

Scatter plot: Attrition probability by age and tenure
Bar chart: Top predictive features (feature importance)
Table: High-risk employees with probability > 0.7
Line chart: Actual vs Predicted attrition rate

Insight:
Low satisfaction and engagement are the top indicators of employee exit. Tenure and training participation also strongly influence attrition probability.

7. Results Summary

The predictive model achieved:

F1 Score: 0.87
Accuracy: 89%

Key Drivers: Engagement, Satisfaction, Tenure, Training Count

The analysis enabled actionable insights for HR teams — including early attrition detection and performance optimization.

8. Key Learnings and Achievements

This project demonstrates the ability to:
Build end-to-end data pipelines integrating SQL, Python, and BI tools.
Design relational data models for business analytics.
Apply machine learning to generate real predictive insights.
Translate technical data into clear, visual business narratives.

It strengthened analytical reasoning, data modeling expertise, and the ability to communicate technical findings through professional storytelling in Power BI.

9. Conclusion

The HR Analytics Dashboard offers a holistic view of workforce performance and attrition behavior, backed by a predictive framework that empowers HR teams to act proactively.
It bridges data engineering, analytics, and AI-driven decision-making — all in one integrated solution.
