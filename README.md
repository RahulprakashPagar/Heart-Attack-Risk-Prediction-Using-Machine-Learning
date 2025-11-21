# Heart-Attack-Risk-Prediction-Using-Machine-Learning
A machine learning project that predicts heart attack risk using Logistic Regression, XGBoost, and KNN, supported by performance analysis, feature importance, and cost-benefit evaluation for healthcare insurance.

# ❤️ Heart Attack Risk Prediction using Machine Learning

This project builds a machine learning-based heart attack risk prediction system to help insurance companies and healthcare providers identify high-risk individuals early.  
It compares Logistic Regression, KNN, and XGBoost models, evaluates recall-focused performance, and includes a real-world cost-benefit analysis demonstrating significant financial savings.

---

## 📊 Project Overview
- **Goal:** Predict heart attack risk using ML to reduce insurance claim losses and enable early health interventions.  
- **Dataset:** Heart Attack Risk Prediction Dataset (CSV Provided)  
- **Files:** Python model code, PDF report, and dataset  
- **Techniques Used:** Logistic Regression, XGBoost, KNN, SMOTE, Feature Engineering  
- **Focus Metric:** **Recall (Sensitivity) — to minimize false negatives**  
- **Author:** [Rahul Pagar](https://www.linkedin.com/in/rahul-pagar1993)

---

## 🧠 Problem Statement
According to the report :contentReference[oaicite:2]{index=2}, traditional insurance screening misses **10% of high-risk individuals**, leading to severe financial losses.  
The objective is to use machine learning to:

- Identify customers at high risk of heart attacks  
- Reduce future insurance claim payouts  
- Enable preventive lifestyle interventions  
- Improve healthcare outcomes and business performance  

---

## ⚙️ Workflow and Methods

### 1️⃣ Data Preparation
Based on the Python file :contentReference[oaicite:3]{index=3}:
- Loaded dataset and cleaned data  
- Split “Blood Pressure” into **Systolic** and **Diastolic**  
- Mapped categorical features to numeric (Sex, Smoking, Diet, etc.)  
- Removed irrelevant fields (e.g., Patient ID, Country)  
- Handled class imbalance using **SMOTE**  
- Standardized numeric features using **StandardScaler**  

### 2️⃣ Model Selection and Evaluation
As detailed in the PDF report :contentReference[oaicite:4]{index=4}:

| Model | Recall | Precision |
|-------|---------|------------|
| Logistic Regression | 0.65 | 0.33 |
| XGBoost | **0.72** | 0.34 |
| KNN | 0.54 | 0.33 |

- **Recall** is prioritized because missing a true heart attack case leads to high medical claim costs.
- **XGBoost** is selected as the best model.

### 3️⃣ Confusion Matrix (XGBoost Results)
From the report’s confusion matrix :contentReference[oaicite:5]{index=5}:

- **TP = 441** → correctly identified high-risk clients  
- **FN = 170** → missed high-risk individuals (critical)  
- **FP = 851** → unnecessary screenings  
- **TN = 291** → correctly identified low-risk clients  

Minimizing **false negatives (FN)** is essential because:

- Missing a high-risk client leads to late-stage health issues  
- Insurance claim payouts increase significantly  

### 4️⃣ Significant Predictors (XGBoost Feature Importances)
As listed in the PDF report :contentReference[oaicite:6]{index=6}:

Top features influencing heart attack risk:

1. **Sleep Hours Per Day – 0.701391**  
2. **Diabetes – 0.103895**  
3. **Systolic BP – 0.068945**  
4. **Physical Activity Days Per Week – 0.066571**  
5. **Diastolic BP – 0.059197**

These features strongly contribute to prediction accuracy.

---

## 💶 Cost-Benefit Analysis (Insurance Use Case)
Detailed in page 5 of the PDF report :contentReference[oaicite:7]{index=7}:

### Without ML Model
- Missed high-risk clients: **876**  
- Cost per claim: **€50,000**  
- Expected claims payout: **€43.8M**  
- Unnecessary tests: **€43.82M**  
- **Total cost = €87.62M**

### With ML Model
- Intervention cost: **€646,000**  
- Claims saved (110 prevented cases): **€5.5M**  
- New claims payout: **€38.3M**  
- ML implementation cost: **€3.5M**  
- **Total cost = €36.94M**

### 💰 Total Annual Savings: **€50.67 Million**  
### 📈 ROI: **751%**

---

## 📈 Insights and Key Findings
- XGBoost provides the **best recall**, crucial for detecting high-risk clients.  
- Sleep hours, diabetes, and blood pressure are major predictors.  
- ML drastically reduces insurance claim losses.  
- High false positives increase test costs but are still cheaper than missed heart attack cases.  
- Early detection improves customer health outcomes and reduces company liabilities.

---

## 📑 Files, Author & Conclusion

### 📁 Files Included
- **`HEART_ATTACK_RISK_PREDICTION_ML APPROCH.pdf`** — Report & Analysis :contentReference[oaicite:8]{index=8}  
- **`ca1_data_mining_heart_attack_risk_prediction.py`** — Full model implementation code :contentReference[oaicite:9]{index=9}  
- **`Heart Attack Risk prediction.csv`** — Source dataset  

### 👨‍💻 Author
**Rahul Pagar**  
🎓 Masters in Business Analytics — Dublin Business School  
🔗 LinkedIn: https://www.linkedin.com/in/rahul-pagar1993

### 🏁 Conclusion
Implementing a machine learning-based heart attack prediction model reduces insurance losses and improves early detection.  
XGBoost delivers the highest recall, making it suitable for healthcare risk assessment.  
The system offers a **€50.67M annual saving** and **751% ROI**, proving the powerful impact of ML in real-world insurance applications.

Future improvements include:
- Boosting precision to reduce unnecessary medical tests  
- Expanding datasets for global applicability  
- Adding neural networks or ensemble models for even better sensitivity  

---
