**ML-Driven Retail Demand Forecasting & Inventory Optimization**

Predicting retail product demand and optimizing inventory for multiple stores using historical sales data with ML regression and actionable recommendations.

🚀 Project Overview

This project leverages retail sales and inventory data to build ML models for demand forecasting and provides inventory optimization recommendations. Using Python, ML algorithms, and an interactive dashboard, stakeholders can make data-driven inventory decisions to reduce stock-outs, minimize overstock, and improve revenue.

📊 Dashboard

Interactive dashboard built in Power BI / Streamlit showcasing:

Daily and weekly sales trends

Stock-out risk heatmaps

Predicted vs actual sales

Reorder recommendations per store & category

KPIs: potential revenue saved, inventory utilization

📦 Dataset Overview

Source: Simulated retail sales & inventory dataset

Total Records: 720 (3 stores × 4 categories × 60 days)

Columns:
date, store_id, product_category, units_sold, inventory_level, price, promotion_flag

🎯 Problem Statement

Retailers often lose revenue due to stock-outs or overstock. The goal is to:

Predict product demand at store & category level

Generate actionable inventory recommendations

Enable managers to make data-backed operational decisions

🧠 Modeling Approach

Models Used: Linear Regression, Random Forest Regressor, Prophet (optional)

Target Variable: units_sold per day

Loss Metric: RMSE (Root Mean Squared Error)

⚙️ Pipeline Summary

✅ Data Preprocessing

Removed duplicates & handled missing values

Converted date formats

Feature encoding for store_id & product_category

✅ Feature Engineering

Lag features (previous day/week sales)

Promotion effect

Stock-out risk indicators

Category-level aggregations

✅ Modeling & Tuning

Applied ML regression models

Cross-validation for accuracy

Feature importance analysis

Forecasted demand converted into inventory recommendations

✅ Inventory Recommendations

Flag products with predicted demand > current inventory

Suggested reorder quantities

Estimated potential lost sales avoided

📁 Repository Structure
retail-demand-ml-inventory/
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_eda_sales_inventory.ipynb
│   ├── 03_demand_forecasting.ipynb
│   ├── 04_inventory_recommendations.ipynb
├── dashboard/
│   ├── retail_dashboard.pbit  # Power BI template
│   ├── retail_dashboard.pdf   # Static version
├── data/
│   └── retail_sales_inventory_dataset.csv
├── README.md
└── requirements.txt

📚 Libraries Used

pandas, numpy, matplotlib, seaborn, scikit-learn, xgboost, prophet

💡 Future Work

Add multi-store regional forecasting

Include seasonal effects (festivals, holidays)

Deployment using Streamlit / FastAPI for interactive dashboards

Explainable AI: SHAP / feature importance for inventory decisions

👤 Author

Aakarsh Kumar Sinha
M.Sc. Operational Research | 2+ years Analytics & Business Consulting
Data Science & ML Enthusiast | Portfolio-Ready Projects for MNCs
