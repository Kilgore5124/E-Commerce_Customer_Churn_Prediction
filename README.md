# 🛍️ E-Commerce Customer Churn Prediction
Predicting customer churn using RFM features and machine learning

This project analyzes customer transaction data from an online retail store to identify churn risks and help businesses retain their most valuable customers using predictive modeling.


## 📑 Table of Contents
- [Overview](#overview)
- [Business Objective](#business-objective)
- [Dataset](#dataset)
- [Process Summary](#process-summary)
- [Key Results](#key-results)
- [How to Run](#how-to-run)
- [Skills Used](#skills-used)
- [Future Improvements](#future-improvements)



## 🧠 Overview

Customer churn is one of the most critical challenges for online retailers. Retaining existing customers is far more cost-effective than acquiring new ones.

In this project, I use real-world transaction data from a UK-based online retailer to:
- Engineer Recency, Frequency, and Monetary (RFM) features
- Build a Random Forest classifier to predict customer churn
- Provide actionable insights to reduce churn risk



## 🎯 Business Objective

The goal is to help the business proactively identify at-risk customers who haven't purchased recently and are likely to churn.

By predicting churn likelihood, the business can:
- Target these customers with retention campaigns
- Personalize offers to high-value clients
- Increase customer lifetime value



## 📦 Dataset

The data is from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Online+Retail).

- Format: Excel file with ~500,000 transactions
- Period: December 2010 to December 2011
- Fields include: `InvoiceNo`, `StockCode`, `Description`, `Quantity`, `InvoiceDate`, `UnitPrice`, `CustomerID`, and `Country`



📝 **How to use:**
1. [Download the dataset here (direct link)](https://archive.ics.uci.edu/ml/machine-learning-databases/00352/Online%20Retail.xlsx)
2. Rename it as: `Online Retail.xlsx`
3. Upload it when prompted in the notebook



## ⚙️ Process Summary

1. **Data Cleaning**
   - Removed cancelled orders, negative prices/quantities, and duplicates
   - Winsorized outliers to reduce noise

2. **Feature Engineering**
   - Calculated RFM metrics (Recency, Frequency, Monetary)
   - Created a binary churn label: no purchase in the last 90 days

3. **Exploratory Data Analysis**
   - Visualized distributions, outliers, and feature relationships with churn

4. **Modeling**
   - Used a Random Forest classifier
   - Evaluated performance with accuracy, AUC, and classification metrics

5. **Insights**
   - Recency was the strongest predictor of churn
   - Churned users had significantly lower frequency and monetary values



## 📊 Key Results

- **Model Accuracy:** 0.86  
- **AUC Score:** 0.89  
- **Most Predictive Feature:** Recency

These results suggest the model is effective at identifying customers at risk of churning, especially those who haven't made recent purchases.



## 🚀 How to Run

You can run the project in [Google Colab](https://colab.research.google.com/) by following these steps:

1. Open the notebook:
2. [E-Commerce_Customer_Churn_Prediction](https://colab.research.google.com/drive/1As99rCaj9oEgE3LRMOX8X8f9meYlywSV?usp=sharing)
3. Download the dataset:
   [Online Retail Dataset](https://archive.ics.uci.edu/ml/machine-learning-databases/00352/Online%20Retail.xlsx)
4. Save it as `Online Retail.xlsx`
5. Upload it when prompted in the notebook



## 🧰 Skills Used

- Python (Pandas, NumPy)
- Data Cleaning & Feature Engineering
- Exploratory Data Analysis (Matplotlib, Seaborn)
- Classification Modeling (Random Forest)
- Model Evaluation (AUC, Confusion Matrix, Classification Report)
- RFM Segmentation
