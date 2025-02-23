![Amazemarketplace cropped](https://github.com/user-attachments/assets/7f1d0d52-e207-4513-883d-dca117adf91b) 

# AmazeMarketplace CLV, Customer Segmentation & RFM Analysis

### Project Overview
As a Data Analyst at AmazeMarketplace, my task is to perform Customer Segmentation using RFM (Recency, Frequency, Monetary) analysis to identify key customer groups and provide actionable insights for the marketing and sales teams.

This project simulates a real-world business scenario where data-driven decisions help improve customer retention, targeted marketing, and overall revenue growth.

##  Project Scope & Objectives
The primary goal is to analyze customer purchasing behavior over a one-year period (2010-12-01 to 2011-12-01) and segment customers into meaningful groups. By leveraging SQL, BigQuery, and data visualization tools (Tableau) I will: 

- Calculate RFM metrics (Recency, Frequency, Monetary) using SQL queries.
- Assign RFM scores (1-4) based on quartiles.
- Identify customer segments, including: Best Customers, Loyal Customers, BigSpenders, Lost Customers, Other segments.
- Develop an interactive dashboard to visualize key insights.
- Provide data-driven recommendations for marketing strategy optimization.
  
### 1. Methodology
#### 1.1 Data Extraction & Preparation
- Use SQL to filter transactions from the dataset for the one-year period (2010-12-01 to 2011-12-01).
- Clean and structure the data for RFM analysis.
#### 1.2 RFM Calculation
- Recency: Time since the last purchase (calculated from 2011-12-01).
- Frequency: Total number of purchases per customer.
- Monetary: Total spending per customer.
#### 1.3 Segmentation & Scoring
- Assign RFM scores (1-4) using APPROX_QUANTILES in SQL.
- Combine RFM scores into a composite score to define customer groups.
#### 1.4 Data Visualization & Insights
- Build a dashboard in Tableau.
- Highlight key customer segments and trends.
- Identify high-value customers for marketing focus.
### 2. Key Business Insights
- What percentage of customers are high-value buyers?
- Which customer group contributes the most revenue?
- How should the marketing team prioritize retention efforts?
### 3. Expected Outcomes
- Optimized marketing strategies based on customer behavior.
- Better customer retention through targeted engagement.
- Revenue growth by focusing on high-value segments.


# Processes for Project Completion
## Phase 1: RFM Analysis (Customer Segmentation)
#### 1. Data Preparation:

![Extract data from amazemarketplace_data_analytics rfm in BigQuery](https://github.com/user-attachments/assets/7d867a50-afef-4db7-b402-7e5674999bd2)
- Extract data from amazemarketplace_data_analytics.rfm in BigQuery.

- Filter data to include only transactions from 2010-12-01 to 2011-12-01.

![Filter data to include only transactions from 2010-12-01 to 2011-12-01](https://github.com/user-attachments/assets/4024674c-e5e2-46eb-b9ae-1118775fc7cf)


## 2. SQL Implementation:
- Use [SQL](https://docs.google.com/spreadsheets/d/14bkNza52kFWUSrScmSLYnQS4Pp0OJ6lh6_VK2Jv_e9M/edit?gid=832667456#gid=832667456)  to calculate Recency, Frequency, and Monetary (RFM) [values](https://docs.google.com/spreadsheets/d/14bkNza52kFWUSrScmSLYnQS4Pp0OJ6lh6_VK2Jv_e9M/edit?gid=40768686#gid=40768686):
- Recency (R): Time since last purchase from 2011-12-01.
- Frequency (F): Number of purchases per customer.
- Monetary Value (M): Total spending per customer.
- Use APPROX_QUANTILES to assign quartiles (1-4) for R, F, and M scores.
  
![Use APPROX_QUANTILES to assign quartiles (1-4) for R, F, and M scores](https://github.com/user-attachments/assets/7aa09b26-f0a5-4c16-b4c6-dfb56dc8b827)


- Merge RFM scores into a single [RFM Score](https://docs.google.com/spreadsheets/d/14bkNza52kFWUSrScmSLYnQS4Pp0OJ6lh6_VK2Jv_e9M/edit?gid=724853351#gid=724853351).
![Merge RFM scores into a single RFM Score](https://github.com/user-attachments/assets/526aa1c9-89c4-4d7e-9c07-dfbb9970db27)

## 3. Customer Segmentation:
Categorize customers into Best Customers, Loyal Customers, Big Spenders, Lost Customers, etc.
![Categorize customers ](https://github.com/user-attachments/assets/dda45596-69b6-467a-995d-424f9bec0a61)

Compare with [rfm_value](https://docs.google.com/spreadsheets/d/14bkNza52kFWUSrScmSLYnQS4Pp0OJ6lh6_VK2Jv_e9M/edit?gid=982402840#gid=982402840) and [rfm_quantiles tables](https://docs.google.com/spreadsheets/d/14bkNza52kFWUSrScmSLYnQS4Pp0OJ6lh6_VK2Jv_e9M/edit?gid=1388210542#gid=1388210542).
![Compare with rfm_quantiles tables](https://github.com/user-attachments/assets/d0a85936-ce9f-4560-a8d6-db0db608f57b)

## 4. Visualization & Insights:
Create a [dashboard in Tableau](https://public.tableau.com/app/profile/kay.afu/viz/CustomerSegmentationRFM_17084114616270/Dashboard1).
![RFM dashboard in Tableau](https://github.com/user-attachments/assets/056a3d50-ce0e-4c1b-8c7e-8cf681edb791)

Provide insights on which customer segment to focus marketing efforts on.
# Phase 2: Customer Lifetime Value (CLV)
### 1. Key Metrics Calculation [(SQL)](https://docs.google.com/spreadsheets/d/14bkNza52kFWUSrScmSLYnQS4Pp0OJ6lh6_VK2Jv_e9M/edit?gid=790783378#gid=790783378):
- registration_week
- revenue_week
- Weekly_revenue.
- Registrations
- Cohort_week
- Total_weekly_revenue
- Weekly_clv
- Customer Lifetime Value (CLV):

![Amazemaketplace_Calculation (SQL)](https://github.com/user-attachments/assets/5b531f94-eaa0-4b33-aab1-f0d4679ad2e4)

![Amazemaketplace_Calculation (SQL)2](https://github.com/user-attachments/assets/a35bffbf-3e62-4e3a-896b-2bc554e88df5)

### 2. [Cohort Analysis for CLV](https://docs.google.com/spreadsheets/d/14bkNza52kFWUSrScmSLYnQS4Pp0OJ6lh6_VK2Jv_e9M/edit?gid=1127414820#gid=1127414820):
- Track customer retention rates over time.
- Identify patterns in repeat purchases.
### 3. Optimization & Business Insights:

![Optimization   Business Insights1](https://github.com/user-attachments/assets/fd6b228b-4fda-42bd-b1e2-0fa9b37cc9e3)

![Optimization   Business Insights2](https://github.com/user-attachments/assets/831be550-9fca-4461-a24a-beac52a86882)

![Optimization   Business Insights3](https://github.com/user-attachments/assets/cf43794c-6f16-444c-8fb9-58b378d4a2ab)

