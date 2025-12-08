# Comparative Analysis of BiLSTM and AfriBERTa for Fake News Detection in Low-Resource Amharic Language

This repository contains the implementation, analysis, and documentation for the project **“Comparative Analysis of BiLSTM and AfriBERTa for Fake News Detection in Low-Resource Amharic Language.”**  
The work compares a tuned BiLSTM architecture with the transformer-based AfriBERTa model for binary fake news detection in the Amharic language.

---

## 1. Project Overview

### Objective
To develop and evaluate deep learning models capable of detecting fake news in the Amharic language, addressing the lack of robust NLP solutions for low-resource linguistic settings.

### Models Examined
- **BiLSTM (Optimized Configuration)**  
  Custom architecture tuned for enhanced generalization and reduced overfitting.
- **AfriBERTa**  
  Transformer-based model adapted from XLM-RoBERTa and fine-tuned for Amharic fake news classification.

### Core Techniques
- Text preprocessing: normalization, cleaning, tokenization, and padding (308-token sequence length)
- Dataset balancing via SMOTE
- Training stabilization using early stopping, learning rate scheduling, and L2 regularization
- Evaluation metrics: Accuracy, Precision, Recall, and F1-Score

---

## 2. Dataset

**Source**  
Hailu, M. (2024). *Amharic Fake News Detection Dataset.*

### Dataset Statistics
- Total samples: 8,630  
- Fake: 4,185  
- Real: 4,445  
- Train/Validation/Test split: 70% / 15% / 15%  
- Padding length: 308 tokens (95th percentile coverage)

---

## 3. Repository Structure

| File | Description |
|------|-------------|
| `Amharic_FakeNews_BiLSTM_AfriBERTa.ipynb` | Implementation of both models |
| `REPORT_Comparative_Analysis.pdf` | Complete technical research report |
| `PPT_Comparative_Analysis.pdf` | Presentation slides |
| `README.md` | Documentation file |

---

## 4. Model Performance

| Model | Accuracy | Precision | Recall | F1-Score | Train–Val Gap |
|-------|----------|-----------|--------|----------|----------------|
| **BiLSTM (Optimized)** | 91.97% | 94.61% | 91.32% | 92.94% | 0.5% |
| **AfriBERTa** | 93.74% | 92.91% | 94.60% | 93.69% | 0.7% |

### Summary
- BiLSTM demonstrates strong performance with lower computational requirements.
- AfriBERTa achieves marginally higher performance due to contextual depth and transfer learning.

---

## 5. Deployment Recommendation

| Model | Suitable Environment | Justification |
|-------|----------------------|---------------|
| **BiLSTM** | Edge / Low-resource systems | Lightweight design, faster inference, minimal hardware requirements |
| **AfriBERTa** | High-compute GPU setups | Highest performance enabled by transformer-based modeling |

---

## 6. Credits

**Contributors**
- Krishna Srikar Manikonda  
- Lingareddy Likhith Reddy  
- Dadam Hemanth Kumar Reddy  

**Institution**  
National Institute of Technology, Puducherry

---

## 7. Acknowledgment

The authors acknowledge **Hailu M.** for providing the Amharic Fake News Detection dataset.

---

## 8. Citation

Manikonda, K. S., Reddy, D. H. K., & Reddy, L. (2025).
Comparative Analysis of BiLSTM and AfriBERTa for Fake News Detection in Low-Resource Amharic Language.
National Institute of Technology, Puducherry.
https://github.com/your-username/Amharic-Fake-News-Detection


---

## 9. Usage Notice

The AfriBERTa implementation contains authenticated access to Hugging Face resources and cannot be made publicly available.  
For research-based access, contact:

**Email:**  
- er.krishnasrikar@gmail.com  
- likhithreddy584@gmail.com
