# COVID-19 Patient Detection & Recommendation System (Symptom-Based)

A **symptom-based COVID-19 detection and recommendation system** built using **supervised machine learning** models to predict suspected COVID-19 cases from **early-stage clinical symptoms**.

> 🎓 **Academic Note:** This project was developed as an **assignment** for the **Machine Learning module** (Part-Time PhD program) at **NIT Silchar**.

---

## 📌 Problem Statement

COVID-19 is highly contagious and early detection is important for timely care and isolation. Many patients initially show **mild symptoms**, making it difficult to detect infections early.

This project aims to build a **recommendation/prediction system** that can predict COVID-19 status from **basic information + common symptoms** using machine learning classifiers.

---

## 🎯 Key Objectives

- Predict COVID-19 test outcome using **symptom-based features**
- Compare multiple ML models and select the best one
- Perform **hyperparameter tuning** to improve performance
- Identify the **most significant symptoms** contributing to prediction 

---

## 📂 Repository Contents

- `corona_detection.ipynb` → Main Jupyter Notebook (training + evaluation)
- `corona_dataset.csv` → Dataset used for training/testing
- `README.md` → Project documentation 
---

## 🧾 Dataset & Features

The dataset contains clinical/basic information of tested individuals and includes **8 key features**:

### ✅ Basic Information
- Gender (Male/Female)
- Age above 60 (True/False)

### ✅ Symptoms (Boolean)
- Cough
- Fever
- Sore throat
- Shortness of breath
- Headache
---

## ⚙️ Approach / Methodology

### 🔹 Data Preprocessing
- Missing value handling (imputation/ignoring based on importance)
- Encoding categorical values using `LabelEncoder`
- Preparing a clean dataset for classification 

### 🔹 Machine Learning Models Used
This project evaluates **six supervised classifiers**:
- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting Machine (GBM)
- XGBoost
- Support Vector Machine (SVM) 

### 🔹 Evaluation Strategy
- **10-Fold Cross Validation**
- Metrics:
  - Accuracy
  - Precision
  - Recall
  - F1-score (F-measure) :contentReference[oaicite:7]{index=7}

---

## 📊 Experimental Results

**Best performing model:** ✅ **SVM**  
**Best accuracy achieved:** ✅ **0.8753 (~87.53%)** 

| Model | Accuracy | Precision | Recall | F1-score |
|------|----------|-----------|--------|----------|
| Logistic Regression | 0.8684 | 0.8664 | 0.8684 | 0.8684 |
| Decision Tree | 0.8729 | 0.8714 | 0.8729 | 0.8729 |
| Random Forest | 0.8726 | 0.8711 | 0.8726 | 0.8726 |
| **SVM (Best)** | **0.8753** | **0.8741** | **0.8753** | **0.8753** |
| GBM | 0.8745 | 0.8730 | 0.8745 | 0.8745 |
| XGBoost | 0.8745 | 0.8730 | 0.8745 | 0.8745 |

---

## 🔍 Most Significant Symptoms (Feature Insight)

From symptom analysis, the most important symptoms/features found were:

✅ **Cough**  
✅ **Headache**  
✅ **Contact with COVID-19 positive patient** 


