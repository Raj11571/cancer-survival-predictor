# cancer-survival-predictor
This project is a machine learning-based approach to predict the survival outcome of lung cancer patients using medical and demographic data. The model is trained on a structured dataset containing health indicators, treatment types, cancer stages, and patient history.

# 🫁 Lung Cancer Survival Prediction Using Machine Learning

## 📌 Project Overview

This project uses machine learning to predict the **survival outcome** of lung cancer patients based on demographic and clinical data. It leverages a Random Forest Classifier to make predictions and evaluate performance.

---

## 🧠 Problem Statement

Predict whether a lung cancer patient will survive, based on factors like age, BMI, smoking history, treatment type, and cancer stage.

---

## 🧾 Dataset Description

Each record includes:

- **Demographics**: Age, Gender, Country  
- **Clinical Info**: BMI, Cholesterol, Comorbidities (Hypertension, Asthma, Cirrhosis, Other Cancer)  
- **Treatment**: Type, Duration  
- **Cancer Info**: Stage  
- **Lifestyle**: Smoking Status, Family History  
- **Outcome**: `survived` (1 = Yes, 0 = No)

---

## ⚙️ Workflow

1. **Data Preprocessing**
   - Handle missing values
   - Compute `treatment_duration` from diagnosis and end treatment dates
   - Drop unnecessary columns
   - One-hot encode categorical features

2. **Model Training**
   - Split dataset
   - Train Random Forest model

3. **Evaluation**
   - Accuracy
   - Classification Report
   - Confusion Matrix

4. **Manual Prediction**
   - Input patient data and get a survival prediction

---

## 🧪 How to Run

```bash
git clone https://github.com/yourusername/lung-cancer-survival-prediction.git
cd lung-cancer-survival-prediction
pip install -r requirements.txt
jupyter notebook lungcancer_code.ipynb
