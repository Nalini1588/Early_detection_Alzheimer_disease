

## Project Overview
This project replicates a published research paper on **early-stage Alzheimer’s disease prediction** using the **OASIS longitudinal dataset**.  
Multiple machine learning models were implemented and evaluated to compare their performance with the results reported in the original paper.

The project focuses on **data preprocessing, exploratory data analysis (EDA), model training, evaluation, and ensemble learning**.

---

## Dataset
- **Dataset Used:** OASIS Longitudinal Dataset (`oasis_longitudinal.csv`)
- **Domain:** Healthcare / Medical Machine Learning
- **Target:** Demented vs Non-demented classification

### Preprocessing Steps
- Handled missing values in **SES** and **MMSE** using median imputation  
- Performed **Exploratory Data Analysis (EDA)** including:
  - Data overview
  - Categorical summary
  - Correlation matrix
- One-hot encoding for categorical feature **Gender (M/F)**
- Train–test split: **80:20**
- **5-fold cross-validation**

---

## Machine Learning Models Implemented
The following models were implemented to replicate the research paper:

- **Decision Tree**
- **Random Forest**
- **Support Vector Machine (SVM)**
- **XGBoost**
- **Voting Classifier (Soft Voting)**

---

## Model Performance (Replication Results)

| Model | Accuracy | F1-Score |
|------|--------|---------|
| Decision Tree | 78.18% | 0.78 |
| Random Forest | **84.55%** | **0.84** |
| SVM | 81.54% | 0.81 |
| XGBoost | 82.20% | 0.82 |
| Voting Classifier | 81.20% | 0.81 |

✔ Random Forest achieved the highest accuracy, consistent with the research paper.

---

## Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Cross-validation scores

---

## Comparison with Original Paper
- Same dataset (OASIS)
- Same ML models
- Similar trends and conclusions
- Minor metric deviations due to:
  - Random state differences
  - Preprocessing variation (MMSE & SES imputation)

---

## Key Learnings
- Hands-on experience with **real-world healthcare datasets**
- Application of ML models in **medical diagnosis**
- Importance of **data preprocessing and reproducibility**
- Practical use of **ensemble learning**
- Evaluation and comparison of ML models using multiple metrics

---

## Technologies Used
- Python
- NumPy
- Pandas
- Scikit-learn
- XGBoost
- Matplotlib
- Seaborn

---

## How to Run the Project
```bash
pip install -r requirements.txt
jupyter notebook
