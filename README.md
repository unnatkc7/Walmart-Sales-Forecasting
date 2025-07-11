

# 🛒 Walmart Sales Forecasting

This project predicts weekly sales for Walmart stores using historical sales data, store characteristics, and external economic factors.

Walmart’s sales data is highly seasonal and influenced by events like holidays. Accurate forecasts help Walmart optimize inventory, staffing, and promotions.



## 📂 Project Overview

- Goal: Predict weekly sales for each store and department.
- Tech Stack: Python, Pandas, scikit-learn, Matplotlib, Seaborn
- Techniques:
  - Exploratory Data Analysis (EDA)
  - Time series features
  - Machine Learning Regression (Random Forest, etc.)
  - Model Evaluation with WMAE



## 📈 Data Sources

- `train.csv` → historical weekly sales
- `test.csv` → weeks to forecast
- `stores.csv` → store types and sizes
- `features.csv` → economic indicators (fuel price, CPI, markdowns, etc.)

Data from the [Walmart Kaggle competition](https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting).



## 💡 Key Features Used

- Store type (A, B, C)
- Store size
- Temperature
- Fuel price
- Markdowns (promotions)
- CPI
- Unemployment rate
- Holiday flag
- Time-based features:
  - Week of year
  - Month
  - Year
  - Lag features:
    - Previous week’s sales
    - Rolling averages

---

## 🔍 Exploratory Data Analysis (EDA)

- Seasonal trends (holidays vs non-holidays)
- Store-level sales variation
- Department-level performance
- Outliers and data quality checks

Example plot:

![Violin Plot](violin_plot.png)

---

## ⚙️ Model Development

### Preprocessing

- Handled missing values
- Created new time-based features
- One-hot encoded categorical variables (`Type`)

### Modeling

- Used Random Forest Regressor
- Evaluated with:
  - RMSE
  - MAE
  




## 📊 Visualizations

- Boxplots of sales by holiday
- Violin plots showing sales distributions
- Time series plots for individual stores
- Feature importance charts



