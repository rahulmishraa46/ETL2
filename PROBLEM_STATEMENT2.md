
# Financial Services Transaction Analysis Assignment

## Problem Statement
To understand customer spending patterns, transaction behaviors, and financial risk factors for a global banking institution using modern data quality tools. Your task is to perform an end-to-end data analysis of credit card transaction records using Python with integrated data validation.

### Dataset
**Source**: [Financial Transactions Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)  
**Records**: 284,807 transactions  
**Time Period**: Two-day transaction window  
**Columns**: 31 (Time, Amount, Class, and 28 anonymized features V1-V28)

## Objectives
1. Perform comprehensive ETL with **data validation** using Perfect
2. Conduct exploratory data analysis (EDA)
3. Generate actionable business insights
4. Create visualizations to support findings
5. Build complete analysis pipeline with **automated quality checks**

## Tasks

### 1. Data Preparation (ETL) with Perfect
-  **a. Extract data with validation**  
  Download dataset using Kaggle API with Perfect schema verification
-  **b. Time conversion with constraints**  
  Convert Time column with Perfect datetime validation  
  `Time >= 0` (non-negative)
-  **c. Clean data with rules**  
  **Perfect Validation Rules**:  
  `Amount > 0` (remove negatives)  
  `Class in [0,1]` (binary fraud indicator)  
-  **d. Calculate metrics with validation**  
  Create Risk Score with Perfect: `@check(risk_score >= Amount)`  
  Add Transaction Size Category with enum validation
-  **e. Save data with quality report**  
  Generate Perfect data quality report  
  Export valid/invalid records separately  
  Load certified data into DuckDB

### 2. Exploratory Analysis
-  **a. Transaction metrics**  
  Total volume with Perfect distribution check  
  Average amount with outlier validation
-  **b. Fraud patterns**  
  Fraud percentage with Perfect confidence interval
-  **c. Time patterns**  
  Hourly distribution with Perfect temporal consistency check
-  **d. Amount analysis**  
  Compare amounts with Perfect statistical significance validation
-  **e. Feature correlation**  
  Identify fraud correlations with Perfect multicollinearity guard


### 4. Business Insights
-  **1. Fraud patterns**  
  Identify high-risk periods with Perfect probability validation
-  **2. High-risk transactions**  
  Determine amount thresholds using Perfect's segmentation analysis
-  **3. Feature importance**  
  Select top features with Perfect's feature impact scoring
-  **4. Transaction patterns**  
  Day/night comparison with Perfect temporal drift detection
-  **5. Value concentration**  
  Top 5% analysis with Perfect Pareto distribution validation



## Submission Requirements
1. **Python Notebook** (`financial_analysis.ipynb`) containing:
   - Complete code with Perfect validations
   - Perfect data quality reports at key stages
   - Embedded visualizations with quality annotations
   - Perfect constraint definitions in YAML/JSON format
```

