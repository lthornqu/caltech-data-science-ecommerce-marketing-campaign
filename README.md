# 📊 Caltech Data Science Project - E-Commerce Marketing Campaign Analysis

---

## 📌 Project Overview
This project is part of a **Caltech Applied Data Science** course, utilizing Python for **exploratory data analysis (EDA), hypothesis testing, and data visualization**. The goal is to analyze customer acquisition and spending behavior across product categories and sales channels. 

We were not given the name or type of store, but based on the products and visualizations, the most likely conclusion is that it is a **wine/liquor store** that also sells some grocery items.

---

## 🏆 Key Objectives
1. **Understand Customer Acquisition & Spending Behavior**
   - Analyze purchasing patterns across different demographics.
   - Assess sales across various channels (store, online, catalog).
   
2. **Conduct Exploratory Data Analysis & Hypothesis Testing**
   - Identify trends using **correlation analysis, regression models, and visualizations**.
   - Detect and treat missing values and outliers.

3. **Provide Insights for Business Strategy**
   - Determine if physical store sales are at risk due to online shopping.
   - Identify the best-selling products.
   - Evaluate the effectiveness of marketing campaigns.

---

## 🛠️ Tools & Technologies Used
- **Python**
- **Pandas**, **NumPy** – Data manipulation
- **Matplotlib**, **Seaborn** – Data visualization
- **Scikit-learn** – Machine learning models (Regression, Correlation Analysis)
- **Statsmodels** – Statistical hypothesis testing

---

## 📝 Dataset Description

The dataset contains **customer information** and **purchasing behavior** from a global e-commerce store.

| Column Name       | Description |
|------------------|------------|
| `ID` | Unique customer identifier |
| `Year_Birth` | Customer's birth year |
| `Education` | Level of education |
| `Marital_Status` | Marital status |
| `Income` | Household income |
| `Kidhome`, `Teenhome` | Number of children in household |
| `Dt_Customer` | Date customer enrolled |
| `Recency` | Days since last purchase |
| `MntWines`, `MntFruits`, `MntMeatProducts`, `MntFishProducts`, `MntSweetProducts`, `MntGoldProds` | Amount spent on different product categories |
| `NumDealsPurchases` | Number of purchases with a discount |
| `NumWebPurchases`, `NumCatalogPurchases`, `NumStorePurchases` | Purchases by sales channel |
| `NumWebVisitsMonth` | Monthly website visits |
| `AcceptedCmp1-5` | Whether the customer accepted a campaign |
| `Response` | Customer response to last campaign |
| `Complain` | Whether the customer has complained |
| `Country` | Customer’s country of residence |

---

## 📊 Steps to Perform

### 🛠 1. Data Cleaning & Preprocessing
- Removed missing values, typos, and inconsistencies.
- Converted **Education & Marital Status** into categorical variables.
- Created new features:
  - **Total Children** (Sum of `Kidhome` & `Teenhome`)
  - **Age** (Derived from `Year_Birth`)
  - **Total Spending** (Sum of all `Mnt` columns)
  - **Total Transactions** (Sum of `NumWebPurchases`, `NumCatalogPurchases`, and `NumStorePurchases`)

- Applied **ordinal encoding** for Education and **one-hot encoding** for categorical variables.

### 📈 2. Exploratory Data Analysis (EDA) & Hypothesis Testing
- Used **correlation matrix heatmaps, scatter plots, bar charts, and violin plots** to analyze customer behavior.
- Conducted **Pearson correlation & regression analysis** to test hypotheses.

### 🎯 3. Business Insights & Key Findings

#### 📌 **Customer Behavior & Sales Trends**
- **Older customers prefer in-store shopping** but are increasingly adapting to online channels.
- **Shopping frequency declines as the number of children increases**, suggesting busier parents have less time to shop.
- **No risk of store sales cannibalization by online channels**—all channels complement each other.

#### 📌 **Sales Performance**
- **Top-selling products:** 🥂 **Wine** (highest revenue), followed by **Meat Products**.
- **Worst-selling products:** 🍎 **Fruit**, followed by **Sweet Products**.
- **U.S. sales are significantly lower than global sales**, with Spain leading in total purchases.

#### 📌 **Marketing Campaign Analysis**
- **Customer age does not significantly influence campaign acceptance.**
- **Spain had the highest campaign acceptance rate.**
- **Higher-educated customers filed more complaints than others.**

---

## 📌 Visualizations & Key Charts
- **Heatmaps** to analyze correlations between customer attributes and spending.
- **Regression models** to predict purchasing behavior.
- **Bar charts** to visualize top-selling products.
- **Scatter & violin plots** to study spending patterns by demographics.

---

## 🚀 How to Use This Project
1. Clone the repository:
   ```bash
   git clone https://github.com/lthornqu/caltech-data-science-ecommerce-marketing-campaign.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Open the **Jupyter Notebook** to explore data and visualize results.

---

## 📌 Future Improvements
- Implement **machine learning models** to predict customer purchasing behavior.
- Conduct **A/B testing** for marketing campaign effectiveness.
- Expand dataset to analyze multiple e-commerce stores.

---

## 👨‍💻 Contributors
- **Lee Thornquist** - Data Analysis & Machine Learning
