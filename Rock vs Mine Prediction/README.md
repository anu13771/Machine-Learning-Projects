# 🪨 Mine vs Rock Classification using Logistic Regression

A Machine Learning project that predicts whether a sonar signal corresponds to a **Rock (R)** or a **Mine (M)** using Logistic Regression.  
This repository contains complete code, dataset details, workflow steps, and model explanation.

---

## 🚀 Project Overview
This project uses the **Sonar Dataset (UCI ML Repository)** to train a binary classification model.

The workflow includes:
- Data Loading
- Exploration & Preprocessing
- Train–Test Split
- Logistic Regression Model Training
- Evaluation
- Prediction System

---

## 📂 Dataset Information
**Name:** Sonar Dataset  
**Source:** UCI Machine Learning Repository  
**Format:** CSV  

- Contains **60 numerical features**
- Target label:
  - **R → Rock**
  - **M → Mine**

Each row represents sonar signal reflections from an object underwater.

---

## 🔍 Project Workflow

### **1️⃣ Importing Dependencies**
Libraries:
- numpy  
- pandas  
- scikit-learn  

---

### **2️⃣ Data Exploration & Processing**
Steps performed:
- Loaded dataset using Pandas  
- Checked structure & summary stats  
- Visualized class distribution  
- Split dataset into features (X) and labels (Y)

---

### **3️⃣ Train-Test Split**
- 90% data for training  
- 10% data for testing  
- Stratified split for balanced class distribution  

---

### **4️⃣ Model Training**
Model used:
- **Logistic Regression**

Training performed using:

model.fit(X_train, Y_train)

---

### **5️⃣ Model Evaluation**
Evaluated using:
- Training accuracy  
- Testing accuracy  
- `accuracy_score()` from scikit-learn  

---

### **6️⃣ Prediction System**
A custom prediction function accepts **60 sonar values** and predicts:

- **🪨 Rock** → R  
- **💣 Mine** → M  

Designed for real-time user inputs.

---

## 📈 Accuracy Summary

| Dataset | Accuracy |
|--------|----------|
| 🏋️ Training | ~83% |
| 🧪 Testing | ~76% |

*(Actual values vary with random state and split)*

---

## 🛠 Requirements

Install required libraries:
pip install numpy pandas scikit-learn

---

### **💡 Use Cases**

This project is perfect for:

Beginners learning Machine Learning

Understanding Logistic Regression

Binary classification practice

Building ML prediction systems
