Customer Churn Prediction — Business Report
1. Executive Summary

This project builds a machine learning–based churn prediction system to identify customers at high risk of leaving the service. Using historical customer behavior data, an XGBoost classifier was trained to estimate churn probabilities and segment customers into actionable risk bands.

The final model achieved strong discriminatory performance and enables targeted retention strategies that can significantly reduce revenue loss.

2. Business Problem

Customer acquisition is significantly more expensive than customer retention. The objective of this project is to proactively identify customers likely to churn so that the business can intervene with personalized retention offers.

3. Dataset Overview

Dataset: Telecom Customer Churn

Records: ~7,000 customers

Features include:

Contract type

Payment method

Tenure

Monthly charges

Service usage

Target variable: Churn (Yes / No)

4. Feature Engineering

Removed unique identifiers (customerID)

Converted categorical variables using one-hot encoding

Converted churn labels to binary (1 = churn, 0 = retained)

Handled missing values in billing data

5. Model Selection

The following models were considered:

Logistic Regression (baseline)

Random Forest

XGBoost (final choice)

XGBoost was selected due to:

Superior ROC-AUC

Ability to model non-linear relationships

Robust handling of feature interactions

6. Model Performance

Final Model Metrics (Test Set):

ROC-AUC: 0.83

Precision (Churn): 0.55

Recall (Churn): 0.72 

Interpretation:

The model correctly identifies ~72% of churners

Precision is acceptable given churn intervention costs

Recall prioritized to minimize missed churners

7. Threshold Optimization

Instead of the default 0.5 threshold, a custom threshold of 0.275 was selected to balance business risk.

At this threshold:

High-risk customers identified: 82

Improved recall without excessive false positives

This aligns with retention-first business strategy.

8. Churn Risk Segmentation

Customers were segmented into three actionable groups:

Risk Band	Probability Range	Business Action
Low	< 0.30	No action
Medium	0.30 – 0.60	Light engagement
High	> 0.60	Retention offers

9. Key Drivers of Churn

Top churn indicators identified:

Short tenure

Month-to-month contracts

High monthly charges

Fiber optic internet service

Electronic check payment method

10. Business Recommendations

Prioritize retention offers for high-risk customers

Incentivize long-term contracts

Target early-tenure customers with onboarding programs

Review pricing strategies for high-charge segments

11. Conclusion

The churn prediction system successfully identifies at-risk customers with strong accuracy and business relevance. Deploying this model can significantly reduce churn-related revenue loss when paired with targeted retention strategies.