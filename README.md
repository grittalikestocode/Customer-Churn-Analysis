# Customer Churn Analysis Project

## Overview
This project analyzes customer churn behavior for a media streaming subscription service. It aims to uncover key churn drivers, develop a predictive model, and present insights through an interactive dashboard. Power BI and Python were used to visualize and model churn likelihood and suggest targeted actions.

## Tools Used
- Python: Pandas, Matplotlib, Seaborn, Scikit-learn, SHAP for model training and interpretability
- Power BI: Dashboard creation (KPI cards, slicers, churn visualizations)

## 📁 Project Structure
~~~
├── Telecom_notebook.ipynb # Jupyter notebook with EDA, modeling, SHAP analysis
├── churn_final.csv # Cleaned dataset used for modeling
├── churn_predictions.csv # Final predictions from Random Forest model
├── dashboard.pbix # Power BI dashboard (3 pages)
├── README.md # Project documentation (this file)
~~~

## 📌 Project Goals

- Analyze churn behavior using customer demographics, billing, and service usage data.
- Build predictive models to identify high-risk customers.
- Use SHAP values for model explainability.
- Deliver interactive Power BI dashboards for stakeholders.

## 🔍 Exploratory Data Analysis (EDA)

Key findings:

- Month-to-month contracts and no support services = higher churn
- Most important features: Tenure, Online Security, Tech Support, Payment Method
- New customers (low tenure) are more likely to churn
- High churn groups: Fiber + Electronic Check + No Tech Support + No Online Security

  
## Modeling Steps
1. Data preprocessing and train-test split
2. Logistic Regression and Random Forest trained and evaluated
3. SHAP explainability applied to Random Forest and Logistic Regressionmodel

Test set Results:

| Metric          | Logistic Regression | Random Forest |
| --------------- | ------------------- | ------------- |
| Accuracy        | 80.0%               | 79.0%         |
| ROC-AUC         | **0.8365**          | 0.8170        |
| F1-score (Yes)  | 0.60                | **0.56**      |
| Recall (Yes)    | **0.57**            | 0.51          |
| Precision (Yes) | 0.64                | 0.63          |
Note: "Yes" class refers to customers who churned.

## Power BI Dashboard (3 Pages)
- Page 1: Churn KPIs and Trends
- Page 2: Services vs Churn
- Page 3: Model outputs (e.g., SHAP summary)


## 💡 Business Recommendations

| Segment                                           | Suggested Action                              |
|---------------------------------------------------|-----------------------------------------------|
| Month-to-month + low usage + no security          | Offer yearly plan discount & bundled security |
| High charges + electronic check + no tech support | Provide payment alternative & upsell support  |
| Basic plan + medium usage                         | Promote feature-rich upgrades                 |

## Final Outputs
- `churn_final.csv`: Cleaned data with engineered features
- `churn_predictions.csv`: Predictions on test set

  
