# Customer Lifetime Value (CLV) Prediction
### An End-to-End Machine Learning System for Predicting Customer Lifetime Value and Enabling Data-Driven Customer Retention

## 📌 Overview
Customer Lifetime Value (CLV) is one of the most important business metrics in customer analytics, representing the total revenue a customer is expected to generate over their relationship with a company. Accurately estimating CLV enables businesses to identify high-value customers, optimize marketing investments, improve customer retention, and make data-driven strategic decisions.

In this project, an end-to-end machine learning pipeline is developed to predict the next 90-day Customer Lifetime Value using historical e-commerce transaction data. The solution includes data preprocessing, customer-level feature engineering, time-based validation to prevent data leakage, model development, and performance evaluation, demonstrating how predictive analytics can support customer retention, marketing optimization, and revenue forecasting in e-commerce.

---
## 🎯 Business Problem

Acquiring new customers is significantly more expensive than retaining existing ones. Businesses therefore need to identify customers who are likely to generate the highest future revenue.

The objective of this project is to predict the next 90-day Customer Lifetime Value (CLV) of each customer using historical transaction data. These predictions can support personalized marketing campaigns, customer segmentation, and more efficient allocation of marketing resources.

---

## 📊 Dataset

This project uses an e-commerce transaction dataset containing historical customer purchase records.

The dataset includes information such as:

- Customer ID
- Invoice Date
- Product Quantity
- Unit Price
- Purchase Amount
- Transaction History

From these raw transactions, customer-level features such as Recency, Frequency, Monetary Value (RFM), Average Order Value, and Purchase Count were engineered for model training.

A time-based cutoff strategy was applied to predict each customer's revenue over the following 90 days while preventing data leakage.

---

## 🛠 Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
---

## ⚙️ Methodology
1. Data Collection and Understanding

2. Data Cleaning and Preprocessing

3. Customer-Level Feature Engineering (RFM Metrics)

4. Exploratory Data Analysis (EDA)

5. Time-Based Train-Test Split

6. Machine Learning Model Development

7. Model Evaluation and Error Analysis

8. Customer Value Segmentation

9. Business Insights and Recommendations
---
## Feature Engineering

Features created include:

- Past Revenue
- Past Transactions
- Recency
- Customer Age
- Average Order Value
- Purchase Frequency

---
## Models Used

- Linear Regression
- Random Forest Regressor
- Gradient Boosting Regressor

---
## Evaluation Metrics

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

Best Tuned Random Forest Results:

- MAE: 1049.67
- RMSE: 7549.55
- R² Score: 0.124

---
## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 📈 Results

The Random Forest Regressor achieved the best overall performance compared to the baseline model on the time-based validation set.

Key outcomes include:

- Accurate prediction of 90-day customer revenue
- Identification of high-value customer segments
- Improved understanding of purchasing behavior through engineered customer-level features
- A reusable machine learning pipeline for future customer value prediction

---

## 🚀 Future Improvements

- Deploy the model using Streamlit and FastAPI
- Add SHAP-based explainability for model predictions
- Compare advanced models such as XGBoost and LightGBM
- Integrate automated retraining pipelines
- Deploy using Docker and cloud services
- Build an interactive business dashboard for marketing teams
