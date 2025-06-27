## 📝 Task 3 Description

> **Build a decision tree classifier to predict whether a customer will purchase a product or service based on their demographic and behavioral data.**  
> The dataset used is the **Bank Marketing dataset** from the **UCI Machine Learning Repository**

This project is part of my ongoing internship where I was assigned to implement a supervised machine learning model using classification techniques. The goal was to use customer-related data to build a **Decision Tree Classifier** that predicts whether a client will subscribe to a term deposit. This task strengthened my understanding of **model-ready preprocessing**, **feature analysis**, and data structure comprehension.

---

## 🗂️ Dataset Overview

The dataset used is `bank-additional.csv` and contains **4,119 rows × 21 columns**. It includes a mix of **categorical and numerical variables**, covering:

### 🔹 Client Profile & Demographics:
- `age`, `job`, `marital`, `education`

### 🔹 Financial & Contact Information:
- `default`, `housing`, `loan`, `contact`, `month`, `day_of_week`

### 🔹 Campaign & Call Outcome:
- `duration`, `campaign`, `pdays`, `previous`, `poutcome`

### 🔹 Economic Indicators:
- `emp.var.rate`, `cons.price.idx`, `cons.conf.idx`, `euribor3m`, `nr.employed`

### 🎯 Target Column:
- `deposit` (originally `y`): Indicates whether the client subscribed to a term deposit (`yes` / `no`)

---

## ✅ Task Breakdown & Performed Operations

### 📌 Data Loading & Exploration
- Loaded the CSV using `pandas`, renamed `y` → `deposit`
- Displayed `.head()`, `.tail()`, `.info()`, `.describe()`
- Verified column data types and structure
- Identified 11 categorical and 10 numerical columns

### 🧹 Data Cleaning
- Checked for missing values using `.isnull().sum()` → ✅ No missing values
- Checked for duplicate rows using `.duplicated().sum()` → ✅ No duplicates

### 🔎 Feature Categorization
- Used `df.select_dtypes()` to separate:
  - `cat_cols` → Categorical features
  - `num_cols` → Numerical features
- Confirmed data readiness for encoding and model training

---

## 📊 Model Preparation 
Although this notebook focuses on **data inspection and preprocessing**, it sets the foundation for the following steps:

- ✅ Encode categorical variables 
- ✅ Split features & target variable
- ✅ Train a `DecisionTreeClassifier` from `sklearn`
- ✅ Evaluate model with metrics like accuracy, confusion matrix, classification report
---

## 🛠️ Tools & Libraries Used

- Python 3
- [Pandas](https://pandas.pydata.org/) for data handling
- [Matplotlib](https://matplotlib.org/) & [Seaborn](https://seaborn.pydata.org/) for visualization
- Jupyter Notebook for step-by-step analysis
- Scikit-learn (to be used in model training)

---

## 📌 Key Learnings

- Practiced working with real-world structured datasets
- Strengthened skills in data analysis, data types, and feature engineering
- Understood how to transition raw CSV files into model-ready datasets
- Gained clarity on the structure and input needs of decision tree classifiers

---

## 🙋‍♀️ Author

**Drashti Parmar**  
🎓 Computer Engineering | 📊 Aspiring Data Scientist  
📬 [LinkedIn Profile](www.linkedin.com/in/drashti-parmar-683358320) <!-- Replace with your actual link -->

---

## 🔗 Acknowledgements

Thanks to my internship mentors and team for assigning this insightful and hands-on task. Their guidance helped me bridge the gap between data analysis and machine learning applications.

---
