# 💼 Income Prediction using Machine Learning

## 📌 Project Overview

This project predicts whether a person earns more than $50K/year based on demographic and employment-related features. The model is trained on the **Adult Census Income Dataset** using a **Random Forest Classifier**.

---

## 🚀 Features

* Data cleaning and preprocessing
* Handling missing values
* Encoding categorical variables using One-Hot Encoding
* Feature selection and importance analysis
* Model training using Random Forest
* Performance evaluation using multiple metrics
* Visualization of top important features

---

## 📂 Dataset

* Dataset used: **Adult Census Income Dataset**
* Contains demographic details such as:

  * Age
  * Workclass
  * Education
  * Marital Status
  * Occupation
  * Race
  * Sex
  * Hours per week
  * Capital gain/loss

---

## ⚙️ Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib, Seaborn

---

## 🧠 Model Used

* **RandomForestClassifier**

  * n_estimators = 100
  * max_depth = 15
  * random_state = 42

---

## 🔄 Data Preprocessing

* Dropped irrelevant columns:

  * `education`, `fnlwgt`, `relationship`
* Replaced `"?"` with NaN and removed missing values
* Label Encoding applied to target variable (`income`)
* One-Hot Encoding applied to categorical features
* Train-test split: 80/20

---

## 📊 Model Performance

| Metric              | Value  |
| ------------------- | ------ |
| Train Accuracy      | 88.56% |
| Test Accuracy       | 85.24% |
| Precision (Class 1) | 0.78   |
| Recall (Class 1)    | 0.57   |
| F1-Score (Class 1)  | 0.66   |

### Confusion Matrix

```
[[4293  240]
 [ 650  850]]
```

---

## 📈 Top 10 Important Features

1. capital.gain
2. marital.status_Married-civ-spouse
3. education.num
4. age
5. marital.status_Never-married
6. hours.per.week
7. capital.loss
8. occupation_Exec-managerial
9. occupation_Prof-specialty
10. marital.status_Divorced

---

## 📉 Visualization

The project includes a barplot showing the top 10 most important features influencing income prediction.

---

### 2. Install dependencies

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

### 3. Run the script

```bash
python main.py
```

---

## ⚠️ Limitations

* Model struggles with recall for high-income class (Class 1)
* No hyperparameter tuning performed
* No cross-validation used
* Dataset imbalance not handled

---

## 🔥 Future Improvements

* Hyperparameter tuning (GridSearchCV / RandomizedSearchCV)
* Handle class imbalance (SMOTE / class weights)
* Try advanced models (XGBoost, LightGBM)
* Deploy model using Flask or FastAPI
* Add cross-validation

---

## 📌 Author

**Satya**

* GitHub: https://github.com/nvm-kai
* LinkedIn: https://www.linkedin.com/in/psatyashry24

---

## ⭐ If you found this useful

Give this repo a star ⭐ and share it!
