Telecom Churn Prediction - A Case Study
This repository explores customer churn prediction in the telecom industry, focusing on identifying high-value customers at risk of churning.

Problem Statement
Business Challenge:

High customer churn rates (15-25%) lead to significant revenue loss.
Acquiring new customers is 5-10x more expensive than retaining existing ones.
Goal:

Develop models to predict churn in high-value customers for proactive retention strategies.
Identify key factors influencing customer churn.
Data and Definitions
Data:

Customer-level data for four consecutive months (June-September) encoded as 6-9.
Dataset available for download: [link to data].
Churn Definition:

Usage-based: No incoming/outgoing calls or mobile internet usage in the fourth month (churn phase).
High-value Customers: Defined by the 70th percentile of average recharge amount in the first two months ("good phase").
Data Preparation
High-Value Customer Filtering:

Select customers exceeding a recharge threshold based on the 70th percentile of average recharge in the "good phase."
This filters down to approximately 30,000 rows.
Churn Labeling and Attribute Removal:

Label churned customers (churn=1) based on usage in the fourth month.
Remove attributes corresponding to the churn phase (those with "_9" suffix).
Modeling Approach
Churn Prediction:
Build models to predict churn in high-value customers for targeted interventions.
Address class imbalance (low churn rate) with appropriate techniques.
Feature Importance Identification:
Develop a separate model (e.g., logistic regression) to identify key churn indicators.
Account for multicollinearity in models like logistic regression.
Evaluation:
Use metrics prioritizing accurate churner identification.
Deliverables
Code for data preparation, modeling, and visualization.
Analysis report with key findings on churn predictors and recommendations for retention strategies.
Further Exploration:

Experiment with different feature engineering techniques.
Investigate alternative classification models.
Implement real-time churn prediction systems
