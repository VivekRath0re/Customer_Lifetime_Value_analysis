# Customer Lifetime Value (CLV) Analysis with Brazilian E-Commerce Public Dataset
This project utilizes a real-world e-commerce dataset from Olist, a Brazilian marketplace, to estimate Customer Lifetime Value (CLV) using advanced modeling techniques. It includes steps for data preprocessing, RFM segmentation, predictive modeling with the MBG/NBD model, and evaluating customer behavior for actionable insights.

# Table of Contents
**Introduction**
**Dataset Overview**
**Objective**
**Methodology**
**Implementation Details**
**Results & Evaluation**
**Conclusion**


# Introduction
Customer Lifetime Value (CLV) quantifies the total worth of a customer to a business over their entire relationship. This metric empowers businesses to optimize acquisition costs and drive strategic growth while ensuring profitability.

This analysis leverages Olist's anonymized e-commerce data (100,000 orders from 2016–2018) to demonstrate how CLV can be calculated, modeled, and interpreted to support decision-making in customer retention and marketing strategies.

Dataset Overview
The project uses the Brazilian E-Commerce Public Dataset by Olist, which includes:

- Orders: Purchase, payment, and delivery information.
- Products: Details about product categories and attributes.
- Reviews: Customer feedback and ratings.
- Customer Data: Location and unique identifiers.
- Marketing Funnel Data: Customer acquisition insights.
- This dataset is ideal for studying the customer lifecycle due to its diversity and granularity.

# Objective
To compute and predict Customer Lifetime Value for Olist's customers, supporting:

- Improved customer segmentation and targeting.
- Strategic insights into marketing expenditure.
- Enhanced operational efficiency and customer retention strategies.
- Methodology
- Data Integration:
- Combine key datasets (Orders, Payments, Customers) to establish a unified transaction log.

# Data Processing:

- Convert timestamps into appropriate date formats.
- Identify unique customers and their transaction histories.


# RFM Analysis:
Perform Recency, Frequency, and Monetary (RFM) segmentation to prepare inputs for CLV modeling.

# CLV Prediction Model:
Train an MBG/NBD Model to predict future customer transactions and evaluate the probability of a customer being active.

# Model Evaluation:

- Fit Accuracy: Compare observed vs. predicted transactions.
- Probability Analysis: Visualize customer activity likelihood over time.
- Cumulative and Incremental Transactions: Assess transaction dynamics over periods.


Implementation Details
Libraries Used
Python: Core programming language.
Pandas: Data manipulation.
NumPy: Numerical operations.
Seaborn & Matplotlib: Visualization.
Lifetimes: CLV modeling.


# Key Steps
1. Data Preprocessing
Integrated orders, customers, and payments datasets.
Filtered valid transaction data with timestamps.
2. RFM Matrix
Created a Recency-Frequency-Monetary (RFM) matrix for customers using calibration_and_holdout_data from the Lifetimes library.
3. MBG/NBD Model
Trained the model with:
Frequency: Number of repeat purchases during the calibration period.
Recency: Time between the first purchase and the last purchase.
T: Total time observed for the customer.
4. Predictions
Forecasted the number of purchases over a 90-day window.
Calculated the probability of each customer being alive based on purchase history.
5. Model Evaluation
Visualized purchase patterns and customer activity probability.
Compared predicted vs. observed transactions for accuracy.
Results & Evaluation



# CLV Predictions:

Accurate forecasts of customer transactions for the next 90 days.
Identified high-value customers and churn risks.
Probability Analysis:

Predicted likelihood of a customer being active today and in the future.
Incremental Insights:

Visualized trends in daily and cumulative transactions, aiding in marketing strategy refinement.
Conclusion
This project successfully demonstrates how CLV can be estimated and leveraged using real-world e-commerce data. Key takeaways include:

High-value customers and churn risks can be identified using predictive models.
CLV provides actionable insights for budget allocation in customer acquisition and retention.
The project can be extended further by incorporating additional data (e.g., marketing funnel metrics) or applying advanced ML techniques for improved accuracy.

