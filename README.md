 🏦 Loan Risk Assessment — German Credit Dataset

A machine learning project that predicts whether a loan applicant is a good or bad credit risk, trained on the classic German Credit Dataset (1,000 real loan cases).

overview of widget : <img width="467" height="528" alt="Loan Risk Assesment" src="https://github.com/user-attachments/assets/65d9d5df-5b1c-4aca-9742-99c8f1affc05" />


---

 📁 Project Structure
loan-risk-assessment/
├── loan_risk_assessment.ipynb   ← Main Colab notebook
├── requirements.txt             ← Python dependencies
├── data/
│   └── german_credit_data.csv   ← Dataset
├── models/
│   └── loan_risk_model.pkl      ← Saved trained model
└── outputs/
    ├── eda_plots.png
    ├── model_evaluation.png
    └── feature_importance.png
    |__ widget 
 📊 Dataset: https://www.kaggle.com/datasets/kabure/german-credit-data-with-risk


Features used
| Feature | Type | Description |
|---|---|---|
| Age | Numeric | Applicant age in years |
| Sex | Categorical | male / female |
| Job | Ordinal | 0 (unskilled) → 3 (highly skilled) |
| Housing | Categorical | own / rent / free |
| Saving Accounts | Ordinal | little → rich |
| Checking Account | Ordinal | little → rich |
| Credit Amount | Numeric | Loan amount in € |
| Duration | Numeric | Loan duration in months |
| Purpose | Categorical | car, education, business, etc. |

---

 🤖 Models Trained

Five models were trained and compared:

| Model | Metric |
|---|---|
| Logistic Regression | AUC scored |
| Decision Tree | AUC scored |
| Random Forest | AUC scored |
| Gradient Boosting | AUC scored |
| XGBoost | AUC scored |

The best performing model is saved to `models/loan_risk_model.pkl`.

---

 🚀 How to Run

. Run Cell 2 and upload `german_credit_data.csv` when prompted
. Click Runtime → Run all
. Use the interactive widget in Cell 11 to test any applicant

---

 📈 Results

- EDA across age, credit amount, duration, housing and purpose
- ROC curves and confusion matrix for all models
- Feature importance chart for the best model
- Interactive widget to assess any custom applicant in real time

---

🛠️ Tech Stack

- Python 3
- Pandas, NumPy
- Scikit-learn
- XGBoost
- Matplotlib, Seaborn
- ipywidgets


