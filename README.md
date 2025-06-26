
## ❤️ Heart Disease Predictor using Logistic Regression

### 📌 Project Overview

This project predicts whether a person is at risk of **heart disease** based on various health and lifestyle 
factors like age, cholesterol, chest pain type, and more.

It is a classic **binary classification problem** where:

* `1` → Has heart disease
* `0` → Does **not** have heart disease

---

### 🧠 Why Logistic Regression?

**Logistic Regression** was chosen because:

* ✅ It is designed for **binary classification**
* ✅ It provides **probabilities**, not just yes/no answers
* ✅ It’s easy to interpret and fast to train
* ✅ It works well when the relationship between features and target is roughly **linear**

---

### 🧪 Dataset Information

* 📄 Source: UCI Heart Disease Dataset
* 🔢 Rows: 303
* 🧬 Features:

  * Age, Sex, Chest Pain Type, Resting BP, Cholesterol
  * Fasting Blood Sugar, Resting ECG, Max Heart Rate
  * Exercise Induced Angina, ST Depression, etc.
* 🎯 Target Column: `output` (0 = No heart disease, 1 = Has heart disease)

---

### 📊 Workflow Followed

```
Load → Clean → Split → Train → Predict → Evaluate
```

#### 1. **Load**

* Data loaded from `heart_disease.csv` using **pandas**

#### 2. **Clean**

* Removed duplicate rows
* Verified data types and checked for null values

#### 3. **Split**

* Used `train_test_split()` from **scikit-learn**
* 80% data used for training, 20% for testing
* `random_state=42` ensures reproducibility

#### 4. **Train**

* Trained a `LogisticRegression` model (`max_iter=1000`) on training data

#### 5. **Predict**

* Model predicts heart disease status for unseen test data

#### 6. **Evaluate**

* Evaluation Metrics:

  * **Accuracy Score**
  * **Confusion Matrix**
  * **Classification Report** (Precision, Recall, F1-Score)

---

### 💡 Learnings

* Logistic Regression is effective for medical binary classification problems.
* Data cleaning (e.g., removing duplicates) impacts model performance.
* Metrics beyond accuracy (like precision and recall) matter in health prediction tasks.

---

### 📁 Libraries Used

* `pandas` — Data loading and manipulation
* `numpy` — Numerical operations
* `scikit-learn` — ML model, train/test split, and evaluation
* `matplotlib` / `seaborn` *(optional)* — Data visualization

---
