# 📧 Spam Mail Detection using Machine Learning

This project builds an ML model that classifies emails as **Spam** or **Ham (Not Spam)** using Natural Language Processing (NLP) and machine learning algorithms.  
The full implementation is available in the notebook:  
`Spam_Mail_Detection_.ipynb`

---

## 🚀 Project Overview

Email spam detection is a classic NLP problem used widely in the real world—Gmail, Outlook, Yahoo Mail, etc.  
This project walks through:

- Data Loading & Cleaning  
- Text Preprocessing (Tokenization, Stopword Removal, Stemming)  
- Feature Extraction using **TF-IDF Vectorization**  
- Model Training (Naive Bayes)  
- Model Evaluation  
- Prediction System to test custom emails  

The goal: classify messages into  
- **0 → Not Spam (Ham)**  
- **1 → Spam**

---

## 📂 Dataset Information

**Dataset:** SMS Spam Collection / Email Spam Dataset  
**Format:** CSV or text file  
**Columns typically include:**  
- `label` — spam/ham  
- `message` — email or SMS text  

**Source:** *(insert your dataset source if needed, e.g., Kaggle/UCI Machine Learning Repository)*  

---

## 🔍 Project Workflow

### **1️⃣ Importing Dependencies**

Libraries used:
- `numpy`  
- `pandas`  
- `nltk` (Natural Language Toolkit)  
- `scikit-learn`  

---

### **2️⃣ Data Exploration & Preprocessing**

Performed tasks:
- Loaded dataset  
- Checked class distribution  
- Cleaned text (removing symbols, numbers, punctuation)  
- Tokenization  
- Stopword removal  
- Stemming using Porter Stemmer  
- Converted text into numerical features using:
  - **TF-IDF Vectorizer**

---

### **3️⃣ Train–Test Split**

- 80% Training  
- 20% Testing  
- Ensured balanced dataset if needed  

---

### **4️⃣ Model Training**

Model used:
- **Multinomial Naive Bayes (NLP-friendly and efficient)**  

Example training code:
model.fit(X_train, y_train)

---

### **5️⃣ Model Evaluation**

Metrics computed:

- Accuracy
- Precision
- Recall
- Confusion Matrix

Typical results:

| Metric | Score |
|--------|----------|
| Accuracy | ~97% |
| Precision | High |
| Recall | High |

---

### **6️⃣ Prediction System**

You can enter any custom message and the model will output:

- Spam
- Not Spam (Ham)

Example:

input_mail = ["Congratulations! You won $1000!!!"]

---

### **🛠 Requirements**

Install necessary libraries:

pip install numpy pandas scikit-learn nltk

---

### **💡 Use Cases**

This project is useful for:

- Beginners learning NLP + machine learning
- Understanding TF-IDF + Naive Bayes
- Email filtering projects
- Real-world spam detection demos
- Deploying a spam classifier using Streamlit / Flask
