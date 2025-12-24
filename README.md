# 🥛 Milk Quality Grading using Explainable Machine Learning

This project develops an end-to-end **machine learning pipeline** to classify milk quality
into **Low**, **Medium**, and **High** grades using physicochemical and sensory attributes.
The project emphasizes **model interpretability** using SHAP, making it suitable for
food safety and quality inspection applications.

---

## 📌 Problem Statement

Milk quality assessment is crucial for consumer safety and dairy processing.
Traditional laboratory testing methods are time-consuming and expensive.

This project aims to:
- Predict milk quality using machine learning
- Handle class imbalance effectively
- Provide explainable predictions suitable for real-world decision-making

---

## 📊 Dataset Description

The dataset contains physicochemical and sensory properties of milk samples.

### Features:
- pH
- Temperature
- Taste
- Odor
- Fat
- Turbidity
- Colour

### Target:
- Grade (Low, Medium, High)

---

## 🔍 Exploratory Data Analysis (EDA)

EDA was performed to:
- Analyze feature distributions
- Identify correlations among numerical features
- Detect class imbalance in the target variable

---

## 🛠 Feature Engineering

Domain-driven features were created to improve model performance:
- **pH × Temperature interaction**
- **Sensory Score** combining Taste, Odor, Fat, and Turbidity

---

## 🤖 Modeling Strategy

A progressive modeling approach was followed:
1. Logistic Regression (Baseline)
2. Support Vector Machine
3. Random Forest
4. XGBoost (Final Model)

---

## ⚖ Handling Class Imbalance

The dataset exhibited class imbalance.
To address this, **SMOTE (Synthetic Minority Oversampling Technique)** was applied
only to the training data using a pipeline.

---

## 📈 Model Evaluation

Models were evaluated using:
- Accuracy
- Precision, Recall, and F1-score
- Confusion Matrix

The final model was selected based on cross-validated performance.

---

## 🔎 Explainable AI (SHAP)

SHAP was used to interpret model predictions:
- **Global Explainability**: Feature importance across the dataset
- **Local Explainability**: Explanation of individual predictions

This enhances transparency and trust in the model’s decisions.

---

## 🧪 Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost
- Imbalanced-learn (SMOTE)
- SHAP
- Matplotlib, Seaborn

---

## 🚀 How to Run the Project

```bash
git clone https://github.com/your-username/milk-quality-ml.git
cd milk-quality-ml
pip install -r requirements.txt
