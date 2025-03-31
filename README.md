
# 🩺 Fetal Health Classification using Machine Learning

This project applies machine learning to classify fetal health status (Normal, Suspect, or Pathological) using Cardiotocogram (CTG) data. The goal is to support early medical intervention and help reduce preventable maternal and neonatal complications.

---

## 📘 Overview

Cardiotocography is a low-cost, non-invasive method for monitoring fetal health. This dataset contains 2,126 CTG readings, each labeled by medical professionals as either:

- **Normal** (1)
- **Suspect** (2)
- **Pathological** (3)

We explore and model this data using two machine learning algorithms: **Random Forest** and **XGBoost**.

---

## 🔍 Objectives

- Clean and explore the CTG dataset
- Train and compare multiple classification models
- Evaluate model performance using precision, recall, F1-score, and confusion matrices
- Identify the most predictive features contributing to fetal risk classification

---

## 📊 Tools & Libraries

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- Scikit-learn
- XGBoost
- Jupyter Notebook

---

## 🤖 Model Performance

| Model          | Accuracy | Suspect F1 | Pathological F1 | Macro F1 |
|----------------|----------|------------|------------------|----------|
| Random Forest  | 93%      | 0.75       | 0.86             | 0.86     |
| XGBoost        | **94%**  | **0.79**   | **0.91**         | **0.89** |

✅ XGBoost slightly outperformed Random Forest, especially in identifying Suspect and Pathological cases.

---

## 🔬 Key Features

The most predictive features included:
- `mean_value_of_short_term_variability`
- `abnormal_short_term_variability`
- `percentage_of_time_with_abnormal_long_term_variability`

These features are aligned with clinical interpretations of fetal distress and heart rate variability.

---

## 📁 Project Structure

```
fetal-health-classification/
│
├── fetal_health.ipynb          # Jupyter Notebook with full workflow
├── README.md                   # Project summary (you are here!)
├── /images                     # Visualizations used in README (optional)
└── requirements.txt            # Python dependencies (optional)
```
#### Data Source: Ayres de Campos et al. (2000) SisPorto 2.0 A Program for Automated Analysis of Cardiotocograms. J Matern Fetal Med 5:311-318 (link)
---

## 📫 Connect with Me

- 💼 [LinkedIn](https://www.linkedin.com/in/travis-moll-4974a21a9)
  
---

## 🧠 Future Improvements

- Add SHAP or LIME for model interpretability
- Deploy model using Streamlit
- Experiment with cross-validation and hyperparameter tuning

---

> *"Improving outcomes through predictive insights — one dataset at a time."*
