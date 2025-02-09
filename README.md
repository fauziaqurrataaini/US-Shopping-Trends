# Customer Shopping Preferences Analysis

### Project Overview

This data analytics project provides valuable insights into consumer behavior and purchasing trends. Understanding these preferences is essential for businesses to optimize their product offerings, marketing strategies, and customer experience. 

### Data Sources

Sales Data : The primary dataset used for this analysis is from Kaggle.com.

### Tools

- Excel - Data Cleaning [Download Here](https://docs.google.com/spreadsheets/d/1S5gKb1fty-aPl1mWNcGQBXVSvSXVs5mCcw3adeqMQvY/edit?usp=sharing)
- Google BigQuery - Data Analysis
- Tableu Public - Data Visualization

### Data Preparation/Cleaning

During the initial data preparation phase, we carried out the following tasks:
1. Loading and examining data
2. Managing missing values
3. Cleaning and formatting the dataset

### Explanatory Data Analysis (EDA)

EDA involved exploring the sales data to answer key question, such as:

- Which product categories are most frequently purchased by active subsribers?
- What is the distribution of payment methods based on total sales and average purchase value?
- What types of products are most purchased by women during winter?
- How do purchases vary across different age groups?
- Which shipping method is most frequently used?

### Data Analysis

Include some interesting code worked with

```sql
SELECT
    Category,
    COUNT(*) AS Total_Transactions,
    AVG(Purchase_Amount_in_USD) AS Avg_Purchase_Amount
FROM `shoppingtrends-450013.dataset_shopping.Shop1`
WHERE
    Subscription_Status = TRUE
GROUP BY Category;
```

### Results

The analysis results are summarized as follows:
- Accessories is the most frequently purchased product by active subsribers.
- The most frequently used payment method contributes the highest to total revenue is Credit Card.
- Products that most purchased by women during winter is shirt, etc.

### Recommendation

Recommendation actions based on the analysis:
- Implement upselling and cross-selling strategies by bundling complementary products.
- Enecouraging high-value payment methods by offering cashback, discounts, or loyalty rewards.
- Stock up on high-demand winter products (shirt) based on female customer's preferences, etc.
