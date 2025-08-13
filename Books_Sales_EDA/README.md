Books Dataset – Data Cleaning, Processing & Exploratory Analysis
This repository contains a complete data cleaning, preprocessing, and exploratory data analysis (EDA) pipeline for a book sales dataset. It demonstrates how to take messy, real-world data and transform it into a structured, analysis-ready format, followed by visual insights.

📊 Project Overview
The dataset Books_Data_Clean.csv consists of book metadata, sales data, author ratings, genres, and publisher details. The project aims to:

Clean irregularities such as missing values, outliers, and invalid entries
Standardize formats for columns like languages, publishing years, and prices
Remove duplicates and ensure consistent data types
Generate EDA visualizations to understand relationships between book features and performance

📂 Dataset Description
Key columns include:

Publishing Year – Year of publication
Book Name – Full title
Author – One or multiple authors
language_code – Book language (e.g., en-US, eng)
Author_Rating – Rating category for the author
Book_average_rating – Average reader rating
Book_ratings_count – Number of reader ratings
genre – Genre category
gross sales – Sales revenue
publisher revenue – Publisher earnings
sale price – Price to customers
sales rank – Ranking in sales charts
Publisher – Publishing company
units sold – Number of copies sold

✨ Data Cleaning Steps

The pipeline performs the following actions:
Import and Inspect
Load with pandas, get structural overview, and check for missing values.
Remove Irrelevant / Invalid Rows
Removed rows with unrealistic publishing years (e.g., -560).
Dropped rows where Book Name was missing.
Duplicate Check
Verified there were no duplicate rows.
Missing Value Strategy
Kept rows with missing language_code to avoid losing crucial data.
Removed rows missing Book Name.
Data Type Verification
Ensured numeric fields (units sold, sales rank, price) have proper data types.
EDA-Prepared Dataset
Created subset-ready clean data to use for visualization and analytics.

📊 Exploratory Data Analysis (EDA)

Generated plots and statistics to discover trends:
Distribution of Publishing Year
Books per Genre (Bar chart)
Top Authors by Average Rating
Boxplot of Book Ratings Count by Genre
Sale Price vs Units Sold (Scatter plot)
Language Distribution (Pie chart)

🛠 Prerequisites

Python 3.10+
pandas
matplotlib
seaborn

▶️ How to Run

Place your raw Books_Data_Clean.csv file in the working directory.
Open and run Books_EDA.ipynb in Jupyter Notebook or JupyterLab.
The notebook will:
Clean/filter data
Prepare plots for EDA
View generated plots directly in the notebook output.

🧹 Key Outcomes

Removed invalid publishing years and necessary missing-value rows.
Dataset free from duplicates and structurally consistent.
Maintained integrity by retaining valuable rows with missing language_code.
Ready-to-use dataset for modeling, reporting, or BI tools.
Plots reveal sales trends, price-value relationships, and genre performance.

👤 Author & Credits
Data Cleaning & Analysis by: [Sabin Shah],contact:sabinshah619@gmail.com

Dataset Source: Kaggle

