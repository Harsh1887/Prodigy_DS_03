# 💼 Decision Tree Classifier – Bank Marketing

A machine learning project designed to predict customer subscription behavior to term deposits using a **Decision Tree Classifier**. The project utilizes the **Bank Marketing dataset** from the UCI Machine Learning Repository and showcases end-to-end data analysis, preprocessing, and model evaluation.

---

## 📌 Overview

This project explores how demographic and behavioral attributes influence a client's likelihood of subscribing to a bank's term deposit. It applies Decision Tree algorithms to model the classification problem and evaluate its performance using standard metrics.

---

## 📊 Dataset Information

- **Source**: [UCI Bank Marketing Dataset](https://archive.ics.uci.edu/ml/datasets/bank+marketing)  
- **Instances**: 41,188 client records  
- **Objective**: Predict the binary target variable `y` — whether the client subscribed to a term deposit (`yes`/`no`)

### 🔑 Key Features

| Feature          | Description                                      |
|------------------|--------------------------------------------------|
| `age`            | Age of the client                                |
| `job`            | Type of job                                      |
| `marital`        | Marital status                                   |
| `education`      | Education level                                  |
| `default`        | Has credit in default?                           |
| `housing`        | Has a housing loan?                              |
| `loan`           | Has a personal loan?                             |
| `contact`        | Contact communication type                       |
| `month`          | Last contact month                               |
| `day_of_week`    | Last contact day of the week                     |
| `duration`       | Duration of last contact in seconds              |
| `campaign`       | Number of contacts during this campaign          |
| `pdays`          | Days since last contact from previous campaign   |
| `previous`       | Number of contacts before this campaign          |
| `poutcome`       | Outcome of the previous marketing campaign       |
| `emp.var.rate`   | Employment variation rate                        |
| `cons.price.idx` | Consumer price index                             |
| `cons.conf.idx`  | Consumer confidence index                        |
| `euribor3m`      | Euribor 3 month rate                             |
| `nr.employed`    | Number of employees                              |
| `y`              | Target variable: subscription status             |

---

## 🧪 Tools & Technologies

- **Language**: Python  
- **Libraries**: Pandas, NumPy, Seaborn, Matplotlib  
- **ML Toolkit**: Scikit-learn (DecisionTreeClassifier)  
- **Environment**: Jupyter Notebook  

---

## 🔁 Project Pipeline

### 1️⃣ Data Preprocessing
- Removed duplicates and handled missing values  
- Categorical features encoded using label encoding  
- Outliers treated using IQR method  

### 2️⃣ Exploratory Data Analysis (EDA)
- Visualized distributions and correlations  
- Generated heatmaps and count plots  
- Derived insights on client behavior patterns  

### 3️⃣ Feature Engineering
- Dropped multicollinear variables (`emp.var.rate`, `euribor3m`, `nr.employed`)  

### 4️⃣ Model Development
- Split dataset into training and testing sets  
- Built two models using:
  - Gini Index
  - Entropy Criterion  

### 5️⃣ Model Evaluation
- Evaluated models using:
  - Accuracy
  - Confusion Matrix
  - Classification Report  
- Plotted Decision Tree for interpretability  

---

## 📈 Performance Metrics

| Criterion | Training Accuracy | Testing Accuracy |
|-----------|-------------------|------------------|
| Gini      | ~93.6%            | ~93.3%           |
| Entropy   | ~93.6%            | ~93.2%           |

---

## ✅ Conclusion

- Both Gini and Entropy performed well with comparable accuracy  
- Gini showed marginally better performance in detecting true positives  
- Decision Tree visualization supports business interpretability  
- Project demonstrates effective application of ML on real-world marketing data  
