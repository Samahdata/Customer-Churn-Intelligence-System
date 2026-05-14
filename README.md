# 📡 Robust Customer Churn Intelligence System
> Predicting telecom customer churn using Machine Learning — Logistic Regression & Decision Tree

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-ML-orange?logo=scikit-learn)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

---

## 📌 Project Overview

This project builds a **Customer Churn Prediction System** for a telecom company using the Telco Customer Churn dataset. The goal is to identify customers who are likely to cancel their subscription, so the business can take proactive retention actions before losing them.

**Key Question:** *Can we predict which customers will leave — and why?*

---

## 🗂️ Repository Structure

```
📦 customer-churn-prediction
 ┣ 📓 Final_Project_Group_10.ipynb   ← Main notebook (full analysis)
 ┣ 📊 Telco_Customer_Churn.csv       ← Dataset
 ┗ 📄 README.md                      ← You are here
```

---

## 🔍 What's Inside the Notebook

| Component | Description |
|-----------|-------------|
| **1. Data Understanding & Preparation** | Explored 33 columns, handled missing values, removed duplicates, fixed inconsistent categories |
| **2. Exploratory Data Analysis (EDA)** | 5 visualizations uncovering churn patterns by contract type, monthly charges, tenure, and tech support |
| **3. Machine Learning Models** | Logistic Regression (baseline) + Decision Tree |
| **4. Assumption Audit** | Documented 3 key assumptions and their risks |
| **5. Model Stress Testing** | Tested robustness across different splits, feature removal, and data subsets |
| **6. Contradiction Analysis** | Found that Contract Type — a strong EDA predictor — was excluded from the model |
| **7. Explainability** | Feature importance analysis with business interpretation |
| **8. Business Recommendations** | 3 actionable strategies to reduce churn |
| **9. Decision Simulation** | Model catches 48.4% of churners by targeting only top 20% highest-risk customers |
| **10. Ethics & Responsible AI** | Bias, fairness, privacy, and model limitations |

---

## 📊 Key Findings

### 🔴 Who is most likely to churn?
- Customers on **Month-to-Month contracts** churn significantly more than yearly subscribers
- Customers paying **$70–$100/month** have the highest churn rate
- **New customers** (< 10 months tenure) are the most at-risk group
- Customers **without Tech Support** churn more than those who have it

### 🤖 Model Performance

| Metric | Logistic Regression | Decision Tree |
|--------|-------------------|---------------|
| Accuracy | 0.797 | ~0.785 |
| Precision | 0.663 | ~0.630 |
| Recall | 0.476 | 0.524 |
| F1 Score | 0.556 | ~0.540 |

> ⚠️ **Note:** Accuracy alone is misleading here due to class imbalance. F1-Score and Recall are the key metrics for this problem.

### 💡 Business Impact
By targeting the **top 20% highest-risk customers**, the model catches **48.4% of all actual churners** — nearly half — without contacting the entire customer base.

---

## 🛠️ Tech Stack

- **Language:** Python 3.x
- **Data Analysis:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn
- **Machine Learning:** Scikit-learn (Logistic Regression, Decision Tree, KNN)
- **Environment:** Jupyter Notebook

---

## ▶️ How to Run

1. Clone the repository:
```bash
git clone https://github.com/Samahdata/Customer-Churn-Intelligence-System.git
```

2. Install dependencies:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

3. Launch the notebook:
```bash
jupyter notebook Final_Project_Group_10.ipynb
```

> Make sure `Telco_Customer_Churn.csv` is in the same folder as the notebook.

---

## 🚀 Future Improvements

- [ ] Add **Correlation Heatmap** to select features based on statistical relationships
- [ ] Include `Contract Type`, `Tech Support`, and `Internet Service` as model features
- [ ] Apply **SMOTE** or class weighting to handle class imbalance
- [ ] Try **Random Forest** or **XGBoost** for better performance
- [ ] Build an interactive **Streamlit dashboard** for real-time churn prediction

---

## 👩‍💻 Author

**Samah Sayed**
📍 Montreal, QC | Vanier College — AEC in Artificial Intelligence & Data Science
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://www.linkedin.com/in/samahsayed55)

---

## 📝 Academic Context

> This project was completed as part of course **420-971-VA — LIA** at Vanier College (30% of final grade).
> AI tools (ChatGPT, Gemini) were used for debugging assistance only, as documented in the AI Usage Log inside the notebook.
