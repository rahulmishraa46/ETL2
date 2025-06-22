# Supermarket Sales Data Analysis Assignment

## Problem Statement
 To understand customer behavior, product performance, and sales patterns to optimize their operations. Your task is to perform an end-to-end data analysis of their sales records using Python.

### Dataset
**Source**: [Supermarket Sales Dataset](https://raw.githubusercontent.com/sushantag9/Supermarket-Sales-Data-Analysis/master/supermarket_sales%20-%20Sheet1.csv)  
**Records**: 1,000 transactions  
**Time Period**: Jan-Mar 2019  
**Columns**: 17 (Invoice ID, Branch, City, Customer type, Gender, Product line, Unit price, Quantity, Tax 5%, Total, Date, Time, Payment, COGS, Gross income, Rating)

## Objectives
1. Perform comprehensive ETL (Extract, Transform, Load) process
2. Conduct exploratory data analysis (EDA)
3. Generate actionable business insights
4. Create visualizations to support findings
5. Build a complete analysis pipeline

## Tasks

### Data Preparation (ETL)
- **a. Extract data from the provided URL**  
  Write a script to download or read the data from its source
-  **b. Handle datetime conversion**  
  Combine Date and Time into a single DateTime column  
  Ensure proper datetime data type
-  **c. Clean data**  
  Standardize text columns (e.g., Title Case)  
  Handle missing/null values
-  **d. Calculate new metrics**  
  Extract Hour of purchase from Time/DateTime  
  Calculate Gross Margin Percentage: `(Gross income / Total) * 100`
-  **e. Save cleaned data**  
  Save as CSV file  
  Save as Parquet file  
  Load into DuckDB database

### Exploratory Analysis
- **a. Revenue metrics**  
  Total revenue (sum of 'Total')  
  Average transaction value (mean of 'Total')
-  **b. Product popularity**  
  Most popular product line by quantity sold
-  **c. Customer satisfaction**  
  City with highest average customer rating
-  **d. Sales patterns**  
  Hourly sales distribution (peak sales hours)
-  **e. Gender analysis**  
  Compare average transaction value by gender

### Business Insights
- **1. Branch performance**  
  Identify highest gross income branch  
  Calculate percentage difference
- **2. Product ratings**  
  Average rating for Electronic Accessories  
  Comparison with other categories
-  **3. Customer value**  
  Revenue comparison: Member vs. Normal customers
-  **4. Sales peaks**  
  Identify busiest day of the week
- **5. Price sensitivity**  
  Correlation between unit price and quantity purchased




