#Customer Shopping Behavior Analysis
End-to-End Data Analytics Solution: Python | SQL | Power BI

## Overview
This project provides a comprehensive analysis of customer shopping behavior using a dataset of 3,900 purchases. The primary objective was to uncover actionable insights regarding spending patterns, customer segmentation, and subscription behavior to guide strategic business decisions. By integrating Python for data engineering, PostgreSQL for deep-dive analysis, and Power BI for visualization, the project identifies key revenue drivers and opportunities for increasing customer loyalty.

## Dataset
Size: 3,900 rows and 18 columns.
Key Features: Customer demographics (Age, Gender, Subscription Status), purchase details (Item, Category, Amount, Season), and behavioral metrics (Discount Applied, Frequency, Review Rating).
Data Quality: Addressed 37 missing values in the Review Rating column.

## Tools & Technologies
Python (Pandas): Data loading, cleaning, and feature engineering.
SQL (PostgreSQL): Advanced querying for business metrics and segmentation.
Power BI: Interactive dashboarding for stakeholder reporting.
Gamma AI: Used for automated report generation and professional presentation of findings.

## Project Steps
1. Data Cleaning & EDA (Python)
Missing Data: Imputed missing review_rating values using the median rating per product category.
Standardization: Renamed columns to snake_case and removed redundant features like promo_code_used.
Feature Engineering: * Created age_group bins (Young Adult, Middle-aged, Adult, Senior).
Calculated purchase_frequency_days.

2. Business Analysis (SQL)
The cleaned data was migrated to PostgreSQL to answer critical business questions:
Revenue Performance: Analyzed revenue by gender (Males generated $157,890 vs. Females at $75,191).
Customer Segmentation: Classified 3,900 customers into Loyal (3,116), Returning (701), and New (83) segments.
Subscription Impact: Compared spending habits, finding that 27% of customers are subscribers.

3. Interactive Dashboard (Power BI)
Developed a dynamic dashboard to visualize KPIs and trends:
Key KPIs: Number of Customers (3.9K), Average Purchase Amount ($59.76), and Average Review Rating (3.75).
Visuals: Revenue by Category (Clothing being the top category), Sales by Age Group, and Subscription Status distribution.

## Key Results & Insights
Top Performers: Jewelry and Blouses are the most purchased items in the Accessories and Clothing categories, respectively.
Age Demographics: Young Adults represent the highest revenue-contributing age group at $62,143.
Shipping Behavior: Express shipping users have a slightly higher average purchase amount ($60.48) than standard shipping users ($58.46).
Product Sensitivity: Items like Hats and Sneakers are highly "discount-dependent," with 50% and 49.66% of their purchases involving discounts.

## Business Recommendations
Boost Subscriptions: Promote exclusive benefits to the 73% of non-subscribers to increase recurring revenue.
Loyalty Programs: Implement rewards specifically for the 701 "Returning" customers to transition them into the "Loyal" segment.
Targeted Marketing: Focus high-impact campaigns on the Young Adult demographic and express-shipping users.

## How to Run
Python: Run the provided notebook to process raw data and generate the cleaned_customer_data.csv.
SQL: Import the CSV into a PostgreSQL database and execute the analysis_queries.sql file.
Power BI: Open the .pbix file and refresh the data source to view the interactive charts.
Report: View the final summary presentation generated via Gamma in the reports/ folder.
