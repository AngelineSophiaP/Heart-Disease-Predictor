
# ❤️ Heart Disease Predictor

This project uses **Machine Learning (Logistic Regression)** to predict whether a person has heart disease based on medical
attributes such as age, cholesterol, resting blood pressure, and more.

## 🧠 Overview

Heart disease is one of the leading causes of death worldwide. Early prediction can help in timely treatment and prevention.
This ML model helps in predicting heart disease using structured patient data.

---

## 📂 Dataset

- **Source**: UCI Machine Learning Repository (Heart Disease Dataset)
- **Format**: CSV file (`heart_disease.csv`)
- **Features**:
  - `age`, `sex`, `cp` (chest pain type)
  - `trestbps` (resting blood pressure)
  - `chol` (serum cholesterol)
  - `fbs` (fasting blood sugar)
  - `restecg`, `thalach`, `exang`, `oldpeak`, `slope`, `ca`, `thal`
  - `output`: **Target variable** (0 = no disease, 1 = disease)

---

## 🔁 Workflow

1. **Load Data** → Using `pandas`
2. **Clean Data** → Drop duplicates
3. **Split Data** → `train_test_split` from `sklearn`
4. **Train Model** → Logistic Regression
5. **Predict** → Run on test set
6. **Evaluate** → Accuracy, Confusion Matrix, Classification Report

---

## 🧪 Libraries Used

```python
import pandas as pd
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LogisticRegression
from sklearn.metrics import accuracy_score, confusion_matrix, classification_report
````

---

## 🚀 How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/heart-disease-predictor.git
   cd heart-disease-predictor
   ```

2. Install dependencies:

   ```bash
   pip install pandas scikit-learn
   ```

3. Run the model:

   ```bash
   python heart_disease_predictor.py
   ```

---

## 📊 Sample Output

```text
✅ Accuracy: 0.85

📊 Confusion Matrix:
[[24  4]
 [ 3 30]]

📄 Classification Report:
              precision    recall  f1-score   support
           0       0.89      0.86      0.87        28
           1       0.88      0.91      0.89        33
```

---

## ✅ Conclusion

This is a simple and interpretable ML solution to predict heart disease. While Logistic Regression was used in this version,
the same dataset can be used to try other models like Random Forest, SVM, or Neural Networks.

---

## 📁 Project Structure

```
heart_disease_predictor/
│
├── heart_disease.csv               # Dataset
├── heart_disease_predictor.py     # Main ML code
├── README.md                       # Project overview (you are here)
```
