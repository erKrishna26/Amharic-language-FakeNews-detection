# Comparative Analysis of BiLSTM and AfriBERTa for Fake News Detection in Low-Resource Amharic Language

This repository contains the code, report, and presentation for the machine learning project **“Comparative Analysis of BiLSTM and AfriBERTa for Fake News Detection in Low-Resource Amharic Language.”**  
The project compares a tuned **BiLSTM model** and a **transformer-based AfriBERTa model** for detecting fake news in the Amharic language, a low-resource African language.

---

## 🧠 Project Overview

**Objective:**  
Develop and evaluate deep learning models for automated fake news detection in the Amharic language, addressing the scarcity of NLP tools for low-resource languages.

**Models Used:**
- **BiLSTM (Sweet Spot Configuration):** Custom-built model optimized through systematic hyperparameter tuning.
- **AfriBERTa:** A transformer-based model fine-tuned from multilingual XLM-RoBERTa for Amharic text.

**Key Techniques:**
- Data preprocessing: cleaning, normalization, tokenization, and padding (308 tokens).  
- SMOTE applied to balance training data.  
- Early stopping, learning rate scheduling, and L2 regularization used for stability.  
- Evaluation metrics: Accuracy, Precision, Recall, F1-score.

---

## 📊 Dataset

**Dataset Source:**  
[Hailu, M. (2024). *Amharic Fake News Detection Dataset*. GitHub Repository.](https://github.com/MenbereHailu/Amharic_Fake_News_Detection_On_Social_Media-_Using_Pretrained-_Language_Model)

**Details:**
- Total samples: 8,630  
- Labels: Fake (4,185) | Real (4,445)  
- Split: 70% Train, 15% Validation, 15% Test  
- Padding length: 308 tokens (95th percentile)  

---

## 🧩 Repository Contents

| File | Description |
|------|--------------|
| `Amharic_FakeNews_BiLSTM_AfriBERTa.ipynb` | Main Jupyter Notebook implementing both models |
| `REPORT_Comparative_Analysis.pdf` | Full technical project report |
| `PPT_Comparative_Analysis.pdf` | Project presentation slides |
| `README.md` | This documentation file |

---

## ⚙️ Model Performance

| Model | Accuracy | Precision | Recall | F1-Score | Train-Val Gap |
|--------|-----------|------------|---------|-----------|----------------|
| **BiLSTM (Sweet Spot)** | 91.97% | 94.61% | 91.32% | 92.94% | 0.5% |
| **AfriBERTa** | 93.74% | 92.91% | 94.60% | 93.69% | 0.7% |


- **Sweet Spot BiLSTM:** Lightweight, interpretable, and resource-efficient.  
- **AfriBERTa:** Superior overall accuracy using transfer learning.

---

## 🚀 Deployment Recommendation

| Model | Best For | Reason |
|--------|-----------|--------|
| **BiLSTM (Sweet Spot)** | Resource-constrained systems | High generalization, simple to deploy |
| **AfriBERTa** | High-performance setups | Leverages pre-trained embeddings for maximum accuracy |

---

## 🏫 Institution and Credits

**Project by:**  
- Krishna Srikar Manikonda (EC23B1026)  

**Under the guidance of:**  
Dr. Venkatesan M. Sundaram  
Associate Professor, Department of Computer Science & Engineering  
National Institute of Technology, Puducherry  

---

## 🙏 Acknowledgments

We thank **Dr. Venkatesan M. Sundaram** for expert guidance and  
**Hailu M.** for providing the Amharic Fake News Detection Dataset.

---

## 🧾 Citation


If you use this project, please cite it as:

Manikonda, K. S.(2025).  
**Comparative Analysis of BiLSTM and AfriBERTa for Fake News Detection in Low-Resource Amharic Language.**  
National Institute of Technology, Puducherry.  
Available at: [https://github.com/your-username/Amharic-Fake-News-Detection](https://github.com/your-username/Amharic-Fake-News-Detection)

