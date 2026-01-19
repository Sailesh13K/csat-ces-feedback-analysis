# 📊 Customer Feedback Analytics — CSAT, CES & Sentiment Classification

This project builds an end-to-end NLP pipeline to analyze customer reviews and predict:

- **CSAT** (Customer Satisfaction)
- **CES** (Customer Effort Score)
- **Sentiment** (Positive / Neutral / Negative)

The models are built using **Multilingual BERT**, trained on real-world e-commerce review data.  
Notebooks cover preprocessing, model training, evaluation, and a unified dashboard.

---

## 🚀 Project Highlights

### 🔍 **Text Classification Tasks**

- **CSAT Prediction** (Satisfied / Neutral / Dissatisfied)
- **CES Prediction** (Easy / Moderate / Difficult)
- **Sentiment Classification** using multilingual BERT

### ⚙️ **Models & Techniques**

- **BERT-based models** (bert-base-multilingual-cased)
- **Class-weighted training** to handle imbalance
- **Confusion matrices + precision, recall, F1-score**
- **Text cleaning pipeline**: lowercasing, punctuation removal, tokenization

### 📊 **Dashboard Notebook**

`FinalDashboard.ipynb` combines:

- Real-time text prediction
- Visual results
- Side-by-side CSAT + CES + Sentiment outputs

(A future Streamlit deployment can be added.)

---

## 📂 Repository Structure

├── CSAT.ipynb # CSAT model training + evaluation
├── CES.ipynb # CES model training + evaluation
├── FinalDashboard.ipynb # Unified prediction & visualization
├── README.md # Project documentation

> **Note:** Trained models are not included to keep the repository lightweight.

---

## 📦 Dataset

This project uses the **Olist Brazilian E-commerce Reviews Dataset**.

📌 Dataset source (Kaggle):  
https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce

### **Dataset Overview**

- ~100,000 customer reviews
- Includes:
  - `review_comment_message`
  - `review_score`
  - `order_id`
- Preprocessed for:
  - CSAT class mapping
  - CES class mapping
  - Sentiment label generation

> The dataset is not uploaded here due to size and licensing.  
> Download it directly from Kaggle using the link above.

---

## 🧠 ML Pipeline

### **1. Data Preprocessing**

- Remove punctuation, emojis, URLs
- Lowercase text
- Tokenization (BERT tokenizer)
- Train/Test split

### **2. Model Training**

- Fine-tuned BERT models
- Class weights to handle imbalance
- AdamW + learning rate scheduling

### **3. Evaluation**

- Accuracy
- Precision, Recall, F1-score
- Confusion Matrix
- Classification Report

---

## 🖥️ Running the Notebooks

1. Download dataset from Kaggle
2. Open any notebook:
   - `CSAT.ipynb`
   - `CES.ipynb`
   - `FinalDashboard.ipynb`
3. Update dataset file path
4. Run all cells to train or test predictions

---
