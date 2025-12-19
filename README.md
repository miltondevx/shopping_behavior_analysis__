# shopping_behavior_analysis__
A Python-based data analysis project examining customer shopping behavior across 3,900+ records to identify revenue patterns, demographic trends, seasonal demand, and actionable business recommendations.
# Customer Buying Behavior Analysis

## Overview
This project analyzes customer purchasing behavior to understand what drives revenue, how demographics influence buying patterns, and where operational improvements can be made. The analysis is based on **3,900+ transaction records** using Python data analysis and visualization libraries.

## Tools & Technologies
- Python
- Pandas
- Matplotlib
- Seaborn

## Dataset
The dataset contains customer demographics, purchase details, payment methods, shipping types, and satisfaction ratings.

Key preprocessing steps:
- Standardized all column names
- Cleaned and normalized data for consistency
- Prepared dataset for downstream analysis and visualization

## Analysis Breakdown

### 1. Demographics Analysis
- Gender distribution across customers
- Age distribution using histograms
- Insight into who the customers are
<img width="1400" height="600" alt="Demographics_Analysis" src="https://github.com/user-attachments/assets/3b8c62d3-20ac-41ac-a89a-26fb67551309" />

### 2. Spending Habits by Category
- Total revenue calculated by product category
- Clothing dominates total sales volume
- Accessories rank second in revenue contribution
<img width="1000" height="500" alt="Spending Habits by Category" src="https://github.com/user-attachments/assets/999be155-f29f-4954-b81f-fafa86af89b0" />

### 3. Seasonal Trends
- Transaction volume analyzed across Spring, Summer, Fall, and Winter
- Fall and Winter show slightly higher purchase frequency
<img width="1000" height="500" alt="Seasonal_Trends" src="https://github.com/user-attachments/assets/5a328e07-5120-4ec1-95eb-6e8dd93eb177" />

### 4. Subscription & Reviews
- Compared review ratings between subscribers and non-subscribers
- No significant difference in satisfaction scores
- Average ratings cluster around **3.7 / 5**
<img width="800" height="600" alt="subscription_ _Reviews" src="https://github.com/user-attachments/assets/83b325cc-7335-4f02-a690-81ddc18abd90" />

### 5. Payment Methods
- Analysis of preferred payment methods
- Credit Card and PayPal are most common for higher-value purchases
- No single dominant payment method overall
<img width="800" height="800" alt="payment_method" src="https://github.com/user-attachments/assets/d55071cd-0964-4afd-bd82-b20a48df8350" />

## Key Findings

1. **Category Dominance**
   - Clothing generates the highest revenue
   - Accessories follow
   - Footwear and Outerwear contribute the least

2. **Demographics**
   - Age distribution is broad and balanced
   - Slight male overrepresentation in transaction count

3. **Seasonality**
   - Sales remain consistent year-round
   - Fall and Winter show marginally higher activity

4. **Subscription Value**
   - Subscription status does not impact review ratings
   - Subscribers and non-subscribers show similar satisfaction levels

5. **Payment Preferences**
   - Highly fragmented payment usage
   - Credit Card, PayPal, Venmo, and Cash used at similar rates

## Actionable Recommendations
- Focus marketing efforts on **high-frequency clothing buyers**
- Convert non-subscribers through incentives such as:
  - Free express shipping
  - Exclusive promotions
- Maintain diverse payment options to support customer preferences

## Sample Code Snippet

```python
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

df = pd.read_csv('shopping_behavior_updated.csv')
df.columns = df.columns.str.replace(' ', '_')
