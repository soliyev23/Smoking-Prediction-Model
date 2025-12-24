# Smoking Status Prediction

This project focuses on predicting **smoking status** using machine learning models based on health-related features.  
An **ensemble approach** combining Logistic Regression and Random Forest is used, with **Optuna** for hyperparameter optimization.

---

## 📊 Dataset

The project uses the following files:

- `train.csv` — training dataset  
- `test.csv` — test dataset  
- `sample_submission.csv` — submission template  

### Target Variable
- Smoking status (binary classification)

### Features
Health-related indicators including:
- Height (cm)
- Weight (kg)
- Systolic blood pressure
- Diastolic blood pressure
- Cholesterol
- HDL
- AST, ALT

Engineered features:
- BMI (Body Mass Index)
- Waist-to-height ratio
- Pulse pressure
- Cholesterol ratio
- Liver enzyme ratio

---

## ⚙️ Tech Stack

- Python  
- pandas, numpy  
- scikit-learn  
- optuna  
- matplotlib, seaborn  

---

## 🧠 Feature Engineering

- BMI and health ratio calculations  
- Polynomial feature generation for nonlinear interactions  
- Standard feature scaling  

---

## 🤖 Models

- **Logistic Regression**
- **Random Forest**
- **Soft Voting Ensemble**

Hyperparameters are optimized using **Optuna**.

---

## 📈 Model Performance

![Learning Curve](learning_curve.png)

Key observations:
- Stable accuracy around **86%**
- Small gap between training and validation curves
- No significant overfitting
- Performance stabilizes after ~4,000 samples

Evaluation metric:
- **ROC-AUC**

---

## 🏆 Final Pipeline

1. Data preprocessing & feature engineering  
2. Train–validation split (80/20)  
3. Hyperparameter tuning with Optuna  
4. Ensemble model training  
5. Prediction on test data  

---

## 📤 Usage

1. Install dependencies:
```bash
pip install pandas numpy scikit-learn optuna matplotlib seaborn
