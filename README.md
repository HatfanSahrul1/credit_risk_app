
# Credit Risk Project

### Live Demo : https://credit-risk-hatfan.streamlit.app/

## Credit Risk Analysis & Modeling (Research)

**Overview:** This repository contains the complete end-to-end Data Science workflow for predicting loan default risk. The project covers Exploratory Data Analysis (EDA), Data Cleaning, handling class imbalance using SMOTE, and comparing Logistic Regression against XGBoost to minimize False Negatives.

### Folder Structure

```text
Credit_Risk_Research/
├── data/
│   ├── cleaned_data.csv
│   ├── loan_data_2007_2014.csv
│   └── ready_to_train.csv
├── model/
│   ├── model_xgb_credit_risk.pkl
│   └── scaler_credit_risk.pkl
├── notebooks/
│   ├── EDA.ipynb
│   ├── data_cleaning.ipynb
│   └── modelling.ipynb
├── LCDataDictionary.xlsx
└── requirements-dev.txt

```

### Model Performance Comparison

| Model | Data Balancing Strategy | Recall (Class 1 / BAD) | Business Impact |
| --- | --- | --- | --- |
| Logistic Regression | SMOTE | 64% | Balanced approach, maintains good loan approval rates. |
| XGBoost (Tuned) | scale_pos_weight | 68% | Prioritizes strict risk management; minimal False Negatives. |

### How to Run

1. Clone this repository to your local machine.
2. Install the dependencies using `pip install -r requirements-dev.txt`.
3. Open Jupyter Notebook and run the notebooks in sequence: `data_cleaning.ipynb` -> `EDA.ipynb` -> `modelling.ipynb`.

---
