# Customer Churn Analysis Project

## Overview
This project investigates why customers of a media streaming subscription service churn and builds a prediction model. 
Power BI and Python were used to visualize and model churn likelihood and suggest targeted actions.

## Tools Used
- SQL: Customer, billing, and usage data extraction
- Python: Pandas, Matplotlib, Seaborn, Scikit-learn, SHAP for model training and interpretability
- Power BI: Dashboard creation (KPI cards, slicers, churn visualizations)

## Modeling Steps
1. Data preprocessing and train-test split
2. Logistic Regression and Random Forest trained and evaluated
3. SHAP explainability applied to Random Forest model

## Key Findings
- Month-to-month contracts and no support services = higher churn
- Most important features: Tenure, Online Security, Tech Support, Payment Method
- High churn groups: Fiber + Electronic Check + No Tech Support

## Power BI Dashboard (3 Pages)
- Page 1: Churn KPIs and Trends
- Page 2: Services vs Churn
- Page 3: Model outputs (e.g., SHAP summary)

## Final Outputs
- `churn_final.csv`: Cleaned data with engineered features
- `churn_predictions.csv`: Predictions on test set
