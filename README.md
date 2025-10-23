# 🩺 Heart Disease Prediction – EDA & Ensemble Modeling

## 📘 Overview
This notebook explores **heart disease prediction** using exploratory data analysis (EDA) and multiple **machine learning algorithms**.  
It demonstrates an end-to-end data science workflow — from cleaning and visualization to model training, evaluation, and ensembling.

---

## ⚙️ Key Steps

### 1. Data Preparation
- Imported essential libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`.
- Cleaned data, handled outliers, and scaled features using `MinMaxScaler`.

### 2. Exploratory Data Analysis (EDA)
- Visualized relationships between clinical variables and target outcome.
- Used:
  - **Heatmaps** for correlation analysis  
  - **Pairplots** for feature relationships  
  - **Distribution plots** for data balance and spread

### 3. Feature Engineering
- Normalized numerical attributes.
- Encoded categorical variables where needed.
- Identified top predictors (age, cholesterol, max heart rate, resting BP).

### 4. Model Building
Implemented and compared:
- Logistic Regression  
- Random Forest  
- Gradient Boosting  
- XGBoost  
- K-Nearest Neighbors  

Evaluation used **train/test split**, **cross-validation**, and **scikit-learn metrics**.

### 5. Ensemble Learning
- Combined models via a **Voting Classifier** to improve performance.
- Compared ensemble accuracy vs individual model scores.

### 6. Model Evaluation
Metrics used:
- Accuracy  
- Precision  
- Recall  
- F1 Score  
- ROC-AUC  

Visuals included:
- **Confusion Matrix**
- **ROC Curves** for model comparison

---

## 📊 Results Summary

| Model | Accuracy | ROC-AUC | Remarks |
|:------|:----------|:--------|:--------|
| Logistic Regression | ~85% | 0.89 | Strong baseline |
| Random Forest | ~91% | 0.93 | Best individual model |
| XGBoost | ~90% | 0.92 | Consistent performer |
| **Ensemble (Voting)** | **92%+** | **0.94+** | Best overall |

---

## 🧠 Insights
- Ensemble model achieved highest stability and accuracy.  
- Normalization significantly improved convergence of gradient-based models.  
- Key risk indicators: **Age**, **Cholesterol**, **Max Heart Rate**, **Resting BP**.

---

## 🧩 Tools & Libraries
`Python` • `pandas` • `numpy` • `matplotlib` • `seaborn` • `scikit-learn` • `xgboost`

---

## 🚀 Run the Project

```bash
pip install -r requirements.txt
jupyter notebook Code.ipynb
