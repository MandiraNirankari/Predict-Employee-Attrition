# Predict-Employee-Attrition
Build a classification model to predict whether an employee is likely to leave a company based on factors such as job satisfaction, salary, work environment, and years of experience.
# 🧠 Employee Attrition Prediction with Random Forest & SMOTE

This repository contains a machine learning project that predicts whether an employee will leave a company based on various HR attributes. The project uses a **Random Forest Classifier** along with **SMOTE (Synthetic Minority Oversampling Technique)** to address class imbalance in the dataset.

---

## 📊 Dataset

- **File:** `6. Predict Employee Attrition.csv`
- **Source:** IBM HR Analytics Dataset (commonly available via Kaggle)
- **Target Variable:** `Attrition`  
  - `Yes` = Employee left  
  - `No` = Employee stayed

---

## 📌 Project Workflow

1. **Data Preprocessing**
   - Dropped non-informative columns:
     - `EmployeeCount`, `Over18`, `StandardHours`, `EmployeeNumber`
   - Encoded categorical columns using `LabelEncoder`

2. **Train-Test Split**
   - 80% training, 20% testing

3. **Balancing Data**
   - Used **SMOTE** to oversample the minority class in training data

4. **Model Training**
   - Applied `RandomForestClassifier` from `scikit-learn`

5. **Evaluation Metrics**
   - Accuracy, Precision, Recall, F1 Score
   - Confusion matrix with a heatmap

---

## 📈 Sample Output (Replace with your actual results)

| Metric     | Score |
|------------|-------|
| Accuracy   | 0.86  |
| Precision  | 0.78  |
| Recall     | 0.72  |
| F1 Score   | 0.75  |

Confusion Matrix:

pip install -r requirements.txt
python predict_attrition.py
├── 6. Predict Employee Attrition.csv      # Dataset file
├── predict_attrition.py                   # Python script for training and evaluation
├── requirements.txt                       # List of dependencies
└── README.md                              # Project documentation
