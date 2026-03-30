# 📄 NLP Contract Risk Analyzer

## 📌 Project Overview
This project is an NLP-based system that analyzes legal contracts to:
- Generate a concise summary of the contract
- Identify and highlight potentially risky clauses

The system uses classical NLP techniques along with machine learning models to perform risk classification and extractive summarization.

---

## 🚀 Features
- 🔍 Clause-level risk detection (Risky / Safe)
- 📑 Extractive contract summarization
- ⚙️ TF-IDF based feature extraction
- 🤖 Multiple ML models (Naive Bayes, Random Forest, XGBoost)
- 🌐 Interactive GUI using Gradio

---

## 🧠 Methodology

### 1. Data Processing
- Dataset used: CUAD (Contract Understanding Atticus Dataset)
- Extracted clause text and clause types
- Assigned risk labels:
  - `1` → Risky clause
  - `0` → Safe clause

---

### 2. Text Preprocessing
- Lowercasing
- Tokenization
- Stopword removal
- Lemmatization
- POS tagging (NLTK / spaCy)

---

### 3. Feature Extraction
- Bag of Words (BoW)
- TF-IDF Vectorization

---

### 4. Model Training
Trained multiple models:
- Naive Bayes
- Logistic Regression
- Random Forest
- XGBoost (Best Performing)

---

### 5. Risk Detection
Each sentence is passed through:
- Preprocessing
- TF-IDF vectorization
- XGBoost model prediction

---

### 6. Extractive Summarization
- Sentence tokenization
- Word frequency calculation
- Co-occurrence matrix (window size = 2)
- Sentence scoring
- Top N sentences selected as summary

---

## 📊 Model Performance
- XGBoost achieved the best accuracy (~90%)
- Balanced precision and recall for risk classification

---

## 🖥️ GUI (Gradio)
- Input: Contract text
- Output:
  - Summary
  - Highlighted risky clauses

---

## 📂 Project Structure
