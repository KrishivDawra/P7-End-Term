# 🏥 AI-Based Health Insurance Premium Prediction

## 📌 Overview

This project builds a **machine learning model** to predict health insurance premiums based on customer health and demographic data.
It simulates a real-world use case for a digital insurance startup (**QuickCover**) aiming to automate premium calculation.

---

## 🎯 Objective

* Replace manual underwriting with **data-driven predictions**
* Improve **accuracy, speed, and scalability**
* Identify key factors influencing insurance premium

---

## 📊 Dataset

* Total Records: **800**
* Features:

  * Age
  * BMI
  * Smoker (Yes/No)
  * Region
  * No_of_Dependents
  * Pre_Existing_Conditions
* Target:

  * **Annual_Premium**

---

## 🔍 Exploratory Data Analysis (EDA)

* Premium distribution is **right-skewed**
* **Smokers** have significantly higher premiums
* **Age and BMI** show positive correlation with premium
* Presence of **outliers** in premium and BMI

---

## ⚙️ Data Preprocessing

* One-Hot Encoding for categorical variables
* Feature scaling (Standardization)
* Train-Test Split (80-20)

---

## 🤖 Models Used

* Linear Regression
* Ridge Regression
* Random Forest Regressor

---

## 📈 Model Performance

| Model             | RMSE  | MAE   | R² Score |
| ----------------- | ----- | ----- | -------- |
| Linear Regression | ~2076 | ~1668 | **0.92** |
| Ridge Regression  | ~2077 | ~1672 | **0.92** |
| Random Forest     | ~2404 | ~1966 | 0.89     |

### 🔥 Insight:

* Linear models performed best → **data is mostly linear**
* Random Forest underperformed due to small dataset and low non-linearity

---

## 📌 Feature Importance

Top factors influencing premium:

* 🚬 **Smoking Status (Highest Impact)**
* 👤 Age
* ⚖️ BMI
* 🏥 Pre-existing Conditions

---

## 📉 Residual Analysis

* Residuals are centered around **zero**
* Indicates **unbiased model predictions**
* Slight presence of large errors (RMSE > MAE)

---

## 🧪 Sample Predictions

| Profile                      | Prediction     |
| ---------------------------- | -------------- |
| Young, non-smoker            | Low premium    |
| Middle-aged, mild conditions | Medium premium |
| Older smoker                 | High premium   |

---

## 💼 Business Impact

* Automates premium calculation
* Reduces manual effort & human bias
* Enables **real-time decision making**
* Scalable solution for insurance companies

---

## ❓ Why RMSE over MAE?

* RMSE penalizes **large errors more**
* Important in insurance where large prediction errors are costly

---

## ⚖️ Ethical Considerations

* Avoid use of sensitive attributes (gender, religion, etc.)
* Ensure fairness and non-discrimination
* Transparent model interpretation

---

## 🚀 Future Improvements

* Add more features (income, lifestyle, medical history)
* Try advanced models (XGBoost, Gradient Boosting)
* Deploy as a web app (Streamlit / API)

---

## 🛠️ Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib, Seaborn

---

## 📁 Project Structure

```
📦 Insurance-Premium-Prediction
 ┣ 📜 insurance_model.ipynb
 ┣ 📊 dataset.csv
 ┣ 📄 README.md
 ┗ 📦 requirements.txt
```

---

## 🙋‍♂️ Author

**Krishiv Dawra**
B.Tech CSE | Chitkara University
Backend Developer | ML Enthusiast

---

## ⭐ If you found this useful, consider giving a star!
