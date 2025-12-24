# marketing-campaign-analysis
Exploratory Data Analysis and Hypothesis Testing on Marketing Campaign Data
# Marketing Campaign Analysis

## 📌 Project Overview
This project performs an end-to-end **Exploratory Data Analysis (EDA)** and **statistical hypothesis testing** on marketing campaign data to understand customer behavior and factors influencing purchases and campaign acceptance.

The analysis is framed around the **marketing mix** (People, Product, Place, Promotion) and aims to derive **business-relevant insights** using data-driven methods.

---

## 🎯 Objectives
- Clean and preprocess real-world marketing data
- Engineer meaningful customer-level features
- Analyze product, channel, and demographic behavior
- Test business hypotheses using statistical methods
- Use appropriate visualizations to support insights

---

## 🧩 Dataset Description
The dataset contains customer demographic information, product spending, purchase channels, and campaign responses.

Key variable groups:
- **People:** Age, Education, Income, Marital Status, Children
- **Product:** Amount spent on wines, meat, fruits, gold, etc.
- **Place:** Store, web, and catalog purchases
- **Promotion:** Campaign acceptances and complaints

---

## 🛠️ Techniques & Concepts Implemented

### 🔹 Data Cleaning
- Fixed inconsistent column names and data types
- Converted date fields to datetime format
- Handled missing income values using **group-wise mean imputation**
  (Education × Marital Status)

### 🔹 Feature Engineering
- Age
- Total number of children
- Total spend across products
- Total purchases across channels

### 🔹 Outlier Treatment
- Applied **Winsorization (1st & 99th percentile)** to handle extreme values
- Preserved all observations while reducing outlier influence

### 🔹 Statistical Hypothesis Testing
- **Pearson Correlation** for behavioral relationships
- **Welch’s t-test** for regional comparison (US vs Rest of World)
- Clear distinction between **statistical significance** and **practical significance**

### 🔹 Data Visualization
- Bar plots for product performance and campaign acceptance
- Boxplots for demographic comparisons
- Scatter plots with regression lines for behavioral patterns
- Heatmaps for correlation analysis

---

## 📊 Key Insights
- Revenue is highly concentrated in **Wines and Meat products**
- **Age alone** does not meaningfully predict campaign acceptance
- Customers with **more children tend to spend less overall**
- Store and online channels show **interaction effects**
- No statistically significant difference in total purchases between
  **US and non-US customers**
- Campaign acceptance varies by country in absolute volume

---

## 🧪 Hypotheses Tested
1. Relationship between age and shopping channel preference  
2. Impact of children on online vs store purchases  
3. Channel cannibalization between store and other channels  
4. Comparison of total purchases: US vs Rest of World  

---

## 🧰 Tech Stack
- **Language:** Python  
- **Libraries:**  
  - pandas  
  - numpy  
  - matplotlib  
  - seaborn  
  - scipy  

---

## 📁 Repository Structure
marketing-campaign-analysis/
│
├── data/
│ ├── marketing_data.csv
│ └── data_dictionary.xlsx
│
├── Notebooks/
│ └── marketing_campaign_analysis.ipynb
│
├── README.md
├── visuals/
  ├── output
  └── output1
  └── output2
  └── output3
  └── output4
  └── output5
  └── output6
