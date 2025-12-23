# Walmart Case Study  
## Gender-Based Purchase Behavior Analysis

---

## Project Overview

Walmart Inc. aims to leverage customer data from the Black Friday sales period to enable data-driven decision-making.  
This case study analyzes whether **customer gender has a statistically significant impact on purchase amount**, helping Walmart design more targeted marketing, inventory, and personalization strategies.

The analysis applies **exploratory data analysis, statistical inference, and confidence interval estimation** to validate business hypotheses using real transaction-level data.

---

## Business Problem Statement

- Walmart wants to understand **customer spending behavior during Black Friday**.
- The primary objective is to analyze the **relationship between customer gender and purchase amount**.
- The business assumes a large customer base consisting of **50 million male and 50 million female customers**.
- Key question:

**Do male and female customers exhibit statistically different spending patterns during Black Friday sales?**

---

## Dataset Description

- **Source**: Walmart Black Friday sales dataset  
- **Rows**: 550,068  
- **Columns**: 10  

### Key Features

| Column Name | Description |
|------------|-------------|
| User_ID | Unique customer identifier |
| Product_ID | Unique product identifier |
| Gender | Customer gender (M/F) |
| Age | Age group of the customer |
| Occupation | Occupation category |
| City_Category | City classification (A, B, C) |
| Stay_In_Current_City_Years | Years in current city |
| Marital_Status | Marital status indicator |
| Product_Category | Product category code |
| Purchase | Purchase amount (target variable) |

- No missing values
- No duplicate records
- Dataset size ~42 MB

---

## Exploratory Data Analysis (EDA)

### Gender Distribution

- Male customers: ~75.3%
- Female customers: ~24.7%

### Purchase Summary by Gender

| Metric | Female | Male |
|------|--------|------|
| Mean Purchase | ~8,735 | ~9,438 |
| Median Purchase | ~7,914 | ~8,098 |
| Standard Deviation | ~4,767 | ~5,092 |
| Max Purchase | ~23,959 | ~23,961 |

Key observations:
- Male customers show **higher average and median purchase values**
- Purchase distributions show variability but a consistent gap between genders

---

## Statistical Approach

### Central Limit Theorem (CLT)

To estimate population-level spending behavior:

- Random samples of **30,000 purchases**
- **1,000 iterations** per gender
- Sampling distributions of the mean constructed

This enables reliable inference even when raw data is not normally distributed.

---

## Confidence Interval Estimation

**95% Confidence Intervals**

### Male Customers
- Mean Purchase CI:  
  **[9,380.64 , 9,496.40]**

### Female Customers
- Mean Purchase CI:  
  **[8,687.94 , 8,782.32]**

### Interpretation
- Confidence intervals **do not overlap**
- Indicates a **statistically significant difference** in average purchase amount

---

## Hypothesis Testing Outcome

- **Null Hypothesis (H₀)**:  
  No difference in average purchase amount between genders.

- **Result**:  
  Null hypothesis **rejected**.

- **Conclusion**:  
  Gender has a **statistically significant impact** on purchase behavior during Black Friday.

---

## Business Recommendations

1. **Target High-Value Male Customers**
   - Promote premium and high-ticket products
   - Focus on electronics and appliances

2. **Increase Female Customer Spend**
   - Personalized discounts and loyalty incentives
   - Bundle offers and value packs

3. **Inventory & Promotion Optimization**
   - Allocate inventory based on gender-driven demand
   - Design targeted promotional strategies

4. **Personalization & Recommendation Systems**
   - Improve recommendation algorithms using gender insights
   - Customize marketing communication channels

5. **Strategic Planning**
   - Apply insights to future sales events
   - Combine gender with age, occupation, and city for deeper segmentation

---

## Final Business Takeaway

The analysis provides strong statistical evidence that **male customers spend more on average during Black Friday sales**.  
By applying these insights, Walmart can:

- Improve revenue forecasting
- Increase marketing ROI
- Enhance customer personalization
- Drive data-backed retail strategies

This case study demonstrates how **statistical analysis and business analytics** translate directly into real-world retail decision-making.
