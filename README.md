# 📉 Customer Churn Prediction using Logistic Regression

AI-ML Assignment 2 | VIT Bhopal University

---

## 🎯 Objective

To build a Logistic Regression model that predicts whether a telecom customer is likely to churn (leave the service) based on their demographic information and service usage patterns.

---

## 📊 Dataset

**Telco Customer Churn Dataset**
- Source: Kaggle
- Link: https://www.kaggle.com/datasets/blastchar/telco-customer-churn
- Records: 7,043 customers
- Features: 21 columns
- Target Variable: Churn (Yes/No)

> **Note:** Dataset is not uploaded to this repository. Please download it from the Kaggle link above and place it in the project folder as `WA_Fn-UseC_-Telco-Customer-Churn.csv`

---

## 📚 Libraries Used

| Library | Purpose |
|---|---|
| `pandas` | Data loading and manipulation |
| `numpy` | Numerical computations |
| `matplotlib` | Data visualization |
| `seaborn` | Statistical plots |
| `sklearn` | Machine learning model and evaluation |
| `warnings` | Suppress unnecessary warnings |

---

## ⚙️ Installation

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

## 🚀 How to Run

**Step 1 — Clone the repository**
```bash
git clone https://github.com/akashyap07/customer-churn-prediction.git
cd customer-churn-prediction
```

**Step 2 — Download the dataset**
```
Go to: https://www.kaggle.com/datasets/blastchar/telco-customer-churn
Download: WA_Fn-UseC_-Telco-Customer-Churn.csv
Place it in the project folder
```

**Step 3 — Run the script**
```bash
python Assignment-2.py
```

---

## 🔬 Methodology

### Task 1 — Data Understanding
- Loaded dataset using Pandas
- Displayed first 5 records
- Identified numerical, categorical, and target features

### Task 2 — Data Preprocessing
- Checked for missing values
- Converted TotalCharges to numeric and filled missing values with median
- Dropped customerID (not useful for prediction)
- Encoded all categorical variables using Label Encoding
- Split dataset into 80% training and 20% testing

### Task 3 — Model Development
- Built Logistic Regression model using scikit-learn
- Trained model on 80% training data
- Predicted churn on 20% test data

### Task 4 — Model Evaluation
- Calculated Accuracy, Precision, Recall and F1 Score
- Generated Confusion Matrix
- Plotted Feature Importance

### Task 5 — Conclusion
- Summarized key findings
- Identified factors influencing churn
- Noted limitations of Logistic Regression

---

## 📈 Results

| Metric | Score |
|---|---|
| Accuracy | ~80% |
| Precision | ~67% |
| Recall | ~57% |
| F1 Score | ~62% |

### Key Observations
1. The model correctly predicted churn with ~80% accuracy
2. Contract type, tenure, and monthly charges are the most influential features
3. Customers on month-to-month contracts are significantly more likely to churn

---

## 📁 Project Structure

```
customer-churn-prediction/
├── Assignment-2.py         ← main Python script
├── README.md               ← project documentation
├── confusion_matrix.png    ← auto generated after running
└── feature_importance.png  ← auto generated after running
```

---

## 📝 Conclusion

The Logistic Regression model achieved ~80% accuracy in predicting customer churn. Key factors influencing churn include contract type, tenure, and monthly charges. A limitation of Logistic Regression is its assumption of linear relationships, which may not fully capture complex churn behavior. Advanced models like Random Forest or XGBoost could improve performance.

