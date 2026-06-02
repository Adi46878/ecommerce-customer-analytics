# E-Commerce Marketing Insights & Customer Analytics

## Project Overview

This project analyzes transactional data from an E-Commerce company to generate marketing insights, understand customer behavior, and build predictive analytics models for business decision-making.

The analysis covers customer acquisition, retention, segmentation, customer lifetime value prediction, cross-selling opportunities, purchase behavior forecasting, and cohort analysis.

---

## Business Objective

The objective of this project is to help the marketing team:

* Monitor key business KPIs
* Understand customer purchasing behavior
* Identify high-value customers
* Improve retention strategies
* Discover cross-selling opportunities
* Predict customer lifetime value
* Forecast future customer purchases
* Evaluate customer retention through cohort analysis

---

## Dataset Description

### Online_Sales.csv

Contains transaction-level sales information.

**Features**

* CustomerID
* Transaction_ID
* Transaction_Date
* Product_SKU
* Product_Description
* Product_Category
* Quantity
* Avg_Price
* Delivery_Charges
* Coupon_Status

### Customers_Data.csv

Contains customer demographic information.

**Features**

* CustomerID
* Gender
* Location
* Tenure_Months

### Discount_Coupon.csv

Contains category-wise discount information.

**Features**

* Month
* Product_Category
* Coupon_Code
* Discount_pct

### Marketing_Spend.csv

Contains daily marketing expenditure.

**Features**

* Date
* Offline_Spend
* Online_Spend

### Tax_Amount.csv

Contains GST information.

**Features**

* Product_Category
* GST

---

## Invoice Value Calculation

Revenue for each transaction was calculated using:

Invoice Value = ((Quantity × Avg_Price) × (1 − Discount_pct) × (1 + GST)) + Delivery_Charges

---

# Project Structure

```text
├── datasets/
│   ├── Online_Sales.csv
│   ├── Customers_Data.csv
│   ├── Discount_Coupon.csv
│   ├── Marketing_Spend.csv
│   └── Tax_Amount.csv
│
├── notebooks/
│   ├── Invoice_Value_Calculation.ipynb
│   ├── Exploratory_Data_Analysis.ipynb
│   ├── Customer_Segmentation_RFM_and_KMeans.ipynb
│   ├── Customer_Lifetime_Value_Prediction.ipynb
│   ├── Cross_Selling_Market_Basket_Analysis.ipynb
│   ├── Next_Purchase_Day_Prediction.ipynb
│   └── Cohort_Analysis_Customer_Retention.ipynb
│
├── outputs/
│   ├── customer_segmentation.csv
│   ├── cluster_summary.csv
│   ├── customer_clv_prediction.csv
│   ├── market_basket_rules.csv
│   ├── next_purchase_prediction.csv
│   └── cohort_retention_analysis.csv
│
└── README.md
```

---

# Project Tasks

## 1. Revenue Calculation

* Calculated invoice value for each transaction
* Applied discounts and GST
* Generated transaction-level revenue metrics

---

## 2. Exploratory Data Analysis (EDA)

Performed detailed analysis including:

* Monthly customer acquisition
* Customer retention analysis
* Revenue from new vs existing customers
* Discount impact analysis
* KPI tracking
* Category-wise performance
* Seasonality and trend analysis
* Marketing spend analysis
* Product performance analysis

### KPIs Analyzed

* Revenue
* Orders
* Customers
* Average Order Value (AOV)
* Quantity Sold
* Marketing Spend
* Delivery Charges
* Tax Contribution

---

## 3. Customer Segmentation

### Heuristic Segmentation (RFM)

RFM metrics:

* Recency
* Frequency
* Monetary Value

Customer groups:

* Premium
* Gold
* Silver
* Standard

### Scientific Segmentation (K-Means)

Performed clustering using:

* Recency
* Frequency
* Monetary Value

Generated customer profiles and segment-specific business strategies.

---

## 4. Customer Lifetime Value Prediction

Built a classification model to categorize customers into:

* Low Value
* Medium Value
* High Value

### Features Used

* Recency
* Frequency
* Quantity Purchased
* Average Order Value

### Model

* Random Forest Classifier

---

## 5. Cross-Selling & Market Basket Analysis

Applied:

* Apriori Algorithm
* Association Rule Mining

### Metrics Used

* Support
* Confidence
* Lift

### Outcomes

* Product Bundling Opportunities
* Frequently Bought Together Products
* Cross-Selling Recommendations

---

## 6. Next Purchase Day Prediction

Predicted when customers are likely to purchase again.

### Classes

* 0–30 Days
* 30–60 Days
* 60–90 Days
* 90+ Days

### Features Used

* Recency
* Frequency
* Revenue
* Quantity
* Average Order Value

### Model

* Random Forest Classifier

---

## 7. Cohort Analysis

Performed customer retention analysis by:

* Grouping customers based on acquisition month
* Measuring month-over-month retention
* Identifying the highest-retention cohorts

### Outputs

* Retention Matrix
* Cohort Heatmap
* Cohort Retention Rates

---

# Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* MLxtend

---

# Key Business Insights

* Identified customer acquisition and retention trends.
* Segmented customers into actionable groups.
* Predicted customer lifetime value.
* Discovered strong cross-selling opportunities.
* Forecasted future purchasing behavior.
* Evaluated customer retention through cohort analysis.
* Generated recommendations for marketing optimization and revenue growth.

---

# Author

**Aditya**

Final Year Engineering Student
Data Analytics & Machine Learning Enthusiast
