# Hospital Readmission Prediction

This project builds a machine learning pipeline to predict hospital readmissions within 30 days using electronic health record (EHR) data from diabetic patients. The goal is to support early intervention and reduce unnecessary readmissions.

---

## Project Summary

- Dataset: [UCI Diabetic Readmission Dataset](https://archive.ics.uci.edu/ml/datasets/diabetes+130-us+hospitals+for+years+1999-2008)
- Records: ~100,000 inpatient encounters
- Target: Whether a patient is readmitted within 30 days

---

## Key Features

- **Data preprocessing**: missing value handling, feature engineering, label encoding
- **Class imbalance handling**: SMOTE (Synthetic Minority Over-sampling Technique)
- **Model training**:
  - Logistic Regression
  - Random Forest
  - XGBoost, LightGBM, CatBoost
- **Evaluation**: ROC-AUC, precision, recall, F1-score
- **Model interpretability**: SHAP values for global and local explanations

---

## Performance

- Final model: **XGBoost**
- **AUC:** 0.71
- **Recall (readmitted patients):** 57%
- SHAP analysis revealed medication count, age, and glucose levels as top predictors.

---

## Files

- `Hospital_Readmission_Enhanced.ipynb` – full notebook with preprocessing, modeling, and analysis
- `Hospital_Readmission_Project_Summary.pdf` – concise project summary for resume/portfolio

---

## Tools & Libraries

`Python`, `Pandas`, `Scikit-learn`, `XGBoost`, `LightGBM`, `CatBoost`, `SHAP`, `Imbalanced-learn`, `Matplotlib`

---

## Use Case

A useful proof-of-concept for hospital systems aiming to prioritize high-risk patients at discharge, reduce penalties due to early readmissions, and improve post-discharge care planning.

---

## License

MIT License.
