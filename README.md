# ecommerce-customer-behavior-analysis
Data analytics case study using Google Sheets, BigQuery, and Tableau.
# E-Commerce Customer Behavior Analysis

## Project Overview
This project analyzes customer demographic and behavioral data from an e-commerce platform.

## Tools Used
- Google Sheets
- Google BigQuery
- Tableau

## Business Questions
- Gender distribution
- Highest income age groups
- Website engagement analysis

## Key Insights
- 26–35 age group is the largest customer segment<img width="1699" height="799" alt="Dashboard 1" src="https://github.com/user-attachments/assets/21febcec-7f79-4ac7-b8a0-a8d0959e0642" />

- High-income users spend more time on site

## Dashboard
https://public.tableau.com/app/profile/rohit.chamlegi/viz/E-commerceCustomerBehaviorAnalysisDashboard_17735893092870/Dashboard1

## Dataset
https://www.kaggle.com/datasets/paulsamuelwe/e-commerce-customer-behaviour-dataset

## Dashboard Preview

<img width="1699" height="799" alt="Dashboard 1" src="https://github.com/user-attachments/assets/b7ccb212-1ca1-4907-949f-11f8e2fd76f9" />

SQL_Queries.sqL
<img width="1920" height="1080" alt="1" src="https://github.com/user-attachments/assets/783973ed-79fa-4223-ad5e-6cb2770d7b99" />

Example SQL query used to analyze gender distribution:
SELECT Gender, COUNT(*) AS customer_count
FROM `casestudy-490307.Ecommerce.customer_info`
GROUP BY Gender
ORDER BY customer_count DESC;

Example SQL query used to analyze gender distribution:
<img width="1920" height="1080" alt="22" src="https://github.com/user-attachments/assets/1cf108ca-39b7-4d19-9f39-06265052d772" />


SELECT `Age Group`, AVG(`Annual Income`) AS avg_income
FROM `casestudy-490307.Ecommerce.customer_info`
GROUP BY `Age Group`
ORDER BY avg_income DESC;

Example SQL query used to analyze average income by age group:
<img width="1920" height="1080" alt="33" src="https://github.com/user-attachments/assets/7d4e4ca0-0788-4599-bde9-3ef860774cd9" />

SELECT `Customer ID`, `Time on Site`
FROM `casestudy-490307.Ecommerce.customer_info`
ORDER BY `Time on Site` DESC
LIMIT 10;
