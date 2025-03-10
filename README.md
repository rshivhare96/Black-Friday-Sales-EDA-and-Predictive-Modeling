# Black Friday Sales EDA and Predictive Modeling

## Overview
This repository contains a comprehensive exploratory data analysis (EDA) and modeling approach on the Black Friday Sales dataset provided by ABC Private Limited. The goal is to understand customer purchase behavior and build a model to predict the purchase amount, enabling personalized marketing offers.

## Dataset Description
- **Source:** ABC Private Limited (Retail company)
- **Contents:**  
  - **Customer Demographics:** Gender, Age, Marital Status, City Category, Stay in Current City, etc.
  - **Product Details:** Product_ID, Product_Category_1, Product_Category_2, Product_Category_3.
  - **Target Variable:** Purchase amount
- **Objective:** To analyze customer behavior and build a predictive model for purchase amounts.

## Data Preprocessing
- **Missing Value Treatment:**  
  - Imputed missing values in `Product_Category_2` and `Product_Category_3` using the mode value grouped by `Age`.
- **Data Cleaning:**  
  - Conducted initial checks on missing values and basic dataset statistics.
- **Feature Engineering:**  
  - Consideration for creating additional features (e.g., count of product categories purchased) to improve model performance.

## Exploratory Data Analysis (EDA)
### Gender Distribution
- **Observation:**  
  - Approximately 400,000 male entries versus around 150,000 female entries.
- **Insight:**  
  - A noticeable imbalance that could impact modeling and should be addressed during the modeling phase.

### Age Distribution
- **Breakdown:**  
  - **26-35:** ~200,000+ records (largest segment)
  - **36-45:** ~100,000+ records
  - **18-25:** ~100,000 records
  - **46-50:** ~50,000 records
  - **51-55:** Slightly under 50,000 records
  - **55+:** ~25,000+ records
  - **0-17:** ~25,000 records
- **Insight:**  
  - The dominant age group is 26-35, indicating a potentially mature, financially active customer segment.

### Purchase Amount Distribution
- **Findings:**  
  - The most frequent purchase amount is around 9,000 (approximately 70,000 occurrences), followed by peaks at 8,000, 6,000, 17,000, and other values.
- **Insight:**  
  - Purchase behavior clusters around specific amounts, suggesting clear spending patterns that can be exploited for targeted promotions.

### Average Purchase Amount by Gender
- **Observation:**  
  - Males average around 9,000, while females average slightly lower at around 8,500.
- **Insight:**  
  - Beyond the higher volume of male transactions, the difference in average purchase amounts may warrant tailored marketing strategies.

## Visualizations
- **Seaborn and Matplotlib:**  
  - Count plots for Gender and Age distribution.
  - Histogram and distribution plots for Purchase amounts.
  - Bar plots to compare average purchase amounts by gender and age.
- **Plotly:**  
  - Interactive histograms showing the relationship between product categories and city segments.
