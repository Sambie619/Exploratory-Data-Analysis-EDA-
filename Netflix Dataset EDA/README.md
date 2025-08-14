Netflix Userbase Data Analysis & Visualization
This project provides data exploration, analysis, and visualization for a synthetic Netflix userbase dataset. Using Python, pandas, matplotlib, and seaborn, it uncovers insights about user demographics, subscription types, revenue patterns, device usage, and country-wise engagement.

📊 Project Overview
The dataset (Netflix Userbase.csv) contains 2,500 user records with the following attributes:

User ID – Unique user identifier
Subscription Type – Basic, Standard, or Premium plan
Monthly Revenue – Revenue from each user (USD)
Join Date – Date the user joined Netflix
Last Payment Date – Date of the latest payment
Country – User's country
Age – User’s age
Gender – Male / Female
Device – Primary device type (Smartphone, Smart TV, Tablet, Laptop)
Plan Duration – Subscription term (1 Month)

The goal is to understand customer patterns to guide retention, marketing, and future business strategies.

✨ Key Analysis Performed

Data Structure & Overview
Loaded CSV data into pandas DataFrame.
Inspected columns, data types, and basic statistics.
Checked for missing values and duplicates (none found).
Descriptive Statistics
Summary of numerical fields: Monthly Revenue, Age, User ID.
Grouping & Aggregation
Average revenue by subscription type
User count by country
Median age by plan duration
Median age by subscription type
Total revenue by gender
Average age by device type
Data Visualization
Scatter plot: Age vs. Monthly Revenue, colored by Gender.
Bar chart: Average Revenue by Country.

📈 Insights Discovered
Revenue by Plan: Premium users generated slightly more average revenue than Basic or Standard.
Country Distribution: USA and Spain had the highest user counts.
Age Patterns: Median age was around 38–39 years across all plans.
Gender-based Revenue: Female users generated slightly more total revenue than male users in this dataset.
Device Patterns: Laptop users were marginally older on average, though differences were minimal.

🛠 Dependencies

Python 3.10+
pandas
matplotlib
seaborn

Install dependencies with:
pip install pandas matplotlib seaborn

📊 Example Visuals

1. Age vs. Monthly Revenue by Gender
Scatter plot showing the relationship between user age and their subscription revenue.
2. Average Revenue by Country
Bar chart ranking countries by average monthly user revenue.

🧹 Data Quality

No Missing Values: All required fields are complete.
Uniform Data Types: Dates are stored as strings but may be converted to datetime for further temporal analysis.
No Duplicates: All users are unique.

👤 Author
Data Analysis & Visualizations by: [Sabin Shah]
Contact: [sabinshah619@gmail.com]

