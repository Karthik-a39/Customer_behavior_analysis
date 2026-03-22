📊 Customer Shopping Behavior Analysis



🧾 1. Project Overview

This project analyzes customer shopping behavior using transactional data from 3,900 purchases across multiple product categories.

The objective is to uncover insights into:

Spending patterns
Customer segments
Product preferences
Subscription behavior

These insights help in making data-driven business decisions.


📂 2. Dataset Summary
Total Rows: 3,900
Total Columns: 18
🔑 Key Features:
Customer Demographics: Age, Gender, Location, Subscription Status
Purchase Details: Item Purchased, Category, Purchase Amount, Season, Size, Color
Shopping Behavior:
Discount Applied
Promo Code Used
Previous Purchases
Frequency of Purchases
Review Rating
Shipping Type
Missing Data:
37 missing values in review_rating
🐍 3. Exploratory Data Analysis (Python)

Data preprocessing and cleaning were performed using pandas:

🔹 Steps:
Data Loading: Imported dataset using pandas
Initial Exploration:
df.info() → structure
df.describe() → statistics
Missing Value Handling:
Filled missing review_rating using median per category
Column Standardization:
Converted column names to snake_case
Feature Engineering:
Created age_group (binning ages)
Created purchase_frequency_days
Data Cleaning:
Checked redundancy between discount_applied and promo_code_used
Dropped promo_code_used
Database Integration:
Loaded cleaned data into MySQL/PostgreSQL using SQLAlchemy


🗄️ 4. Data Analysis (SQL)


Performed business-level analysis using SQL:
📌 Key Business Questions:
Revenue by Gender
High-Spending Discount Users
Top 5 Products by Rating
Shipping Type Comparison
Subscribers vs Non-Subscribers Analysis
Top Discounted Products
Customer Segmentation
New
Returning
Loyal
Top 3 Products per Category
Repeat Buyers vs Subscription
Revenue by Age Group

📊 5. Dashboard (Power BI)

An interactive dashboard was built to visualize:
Revenue trends
Customer segmentation
Product performance
Subscription insights
🔹 Key Visuals:
Revenue by Gender
Category-wise Sales
Subscription Impact
Age Group Analysis
Top Products


💡 6. Business Recommendations


Based on analysis:
Boost Subscriptions
→ Offer exclusive benefits and discounts
Customer Loyalty Programs
→ Convert repeat buyers into loyal customers
Optimize Discount Strategy
→ Balance revenue and profit margins
Product Positioning
→ Promote top-rated and high-selling products
Targeted Marketing
→ Focus on high-revenue age groups and premium customers

🚀 7. Tech Stack

Python (pandas, data cleaning)
SQL (MySQL/PostgreSQL) (analysis)
Power BI (dashboard & visualization)

🔥 8. Project Pipeline

CSV Data → Python (Cleaning & EDA) → SQL (Analysis) → Power BI (Dashboard)


🧠 9. Key Learnings

Data cleaning and preprocessing
Writing advanced SQL queries (CTE, window functions)
Building end-to-end data pipelines
Creating business dashboards

📌 10. Future Improvements
Add real-time data pipeline
Use large datasets for scalability
Integrate with backend APIs
Deploy dashboard online
