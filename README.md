# Amazon Pricing and Discount Analysis

Statistical analysis of Amazon product data to examine relationships between pricing, discounts, product categories, and customer ratings.

## Project Overview

This project analyses the relationship between product pricing, discount percentages, product categories, and customer ratings using the Amazon Sales Dataset.

The analysis covers data cleaning, exploratory data analysis, descriptive statistics, correlation analysis, ANOVA, and regression analysis to identify patterns in pricing and customer ratings.

## Dataset

- Dataset: Amazon Sales Dataset
- Source: Kaggle
- Records: 1,465
- Cleaned records used for analysis: 1,464
- Key variables: Actual Price, Discounted Price, Discount Percentage, Customer Rating, Rating Count, and Product Category

### Dataset

[View Amazon Sales Dataset](https://www.kaggle.com/datasets/karkavelrajaj/amazon-sales-dataset)

## Data Cleaning and Preprocessing

The following preprocessing steps were performed:

- Converted price, rating, and rating count fields to numeric format
- Removed currency symbols and comma formatting from price fields
- Converted discount percentage values to numeric form
- Calculated discount percentage for verification
- Consolidated hierarchical product categories into five broad categories
- Removed records with missing or invalid values in key analytical variables
- Retained price outliers for full-dataset analysis while limiting their effect on visual interpretation

## Exploratory Data Analysis

The analysis includes:

- Actual price distribution
- Discount percentage distribution
- Customer rating distribution
- Average rating by product category
- Average discount by product category
- Discount percentage vs. customer rating
- Actual price vs. customer rating
- Pearson correlation heatmap
- Customer rating distribution by category
- Average rating by discount bracket

All visualizations are included in the project notebook.

## Statistical Analysis

The following statistical methods were applied:

- Pearson correlation
- Spearman correlation
- One-way ANOVA
- Pairwise t-tests with Bonferroni adjustment
- Simple linear regression
- Multiple linear regression
- Discount-bracket ANOVA

## Key Findings

- Discount percentage and customer rating showed a weak negative correlation (Pearson r = -0.156).
- Actual price and customer rating showed a weak positive correlation (Pearson r = 0.123).
- Actual price and discount percentage showed a weak negative correlation (Pearson r = -0.118).
- Customer ratings differed significantly across product categories (ANOVA F = 13.96, p < 0.001).
- Simple regression showed that discount percentage explained approximately 2.4% of the variation in customer ratings (R² = 0.024).
- A multiple regression model using actual price, discount percentage, and rating count explained approximately 4.7% of rating variation (R² = 0.047).
- Discount-bracket ANOVA could not provide a meaningful comparison because the observations were highly imbalanced across brackets.

## Tools and Technologies

- Python
- Pandas
- NumPy
- SciPy
- Matplotlib
- Seaborn
- Jupyter / Google Colab

## Repository Contents

```text
amazon-pricing-discount-analysis/
│
├── README.md
├── Amazon_Pricing_Discount_Analysis.ipynb
└── requirements.txt
```

## Notebook

[View Complete Notebook](./BDM_Analysis.ipynb)

## Detailed Report

[View Detailed Report](./Amazon_Pricing_Discount_Analysis_Report.pdf)
