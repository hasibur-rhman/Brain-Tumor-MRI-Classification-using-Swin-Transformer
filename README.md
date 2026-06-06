# 🧠 Brain Tumor MRI Classification using Swin Transformer

## 📌 Overview

This project implements a **Multi-Stage Swin Transformer** model for brain tumor classification from MRI images.  
The model classifies brain MRI scans into four categories:

- Glioma  
- Meningioma  
- No Tumor  
- Pituitary Tumor  

It uses a custom-built Swin Transformer architecture with **window-based self-attention**, **shifted windows**, and **patch merging** for hierarchical feature learning.

---

## 🚀 Key Features

- 🔷 Custom implementation of Swin Transformer from scratch (PyTorch)
- 🔷 Multi-stage hierarchical architecture
- 🔷 Window-based Multi-Head Self Attention (W-MSA)
- 🔷 Shifted window mechanism for cross-window interaction
- 🔷 Patch merging for feature downsampling
- 🔷 Cosine Annealing Warm Restarts scheduler
- 🔷 Data augmentation for improved generalization
- 🔷 Full training pipeline with metrics tracking

---

## 🧠 Model Architecture

The model consists of:

- Patch Embedding Layer  
- Swin Transformer Stages (4 stages)  
- Window Attention Blocks  
- Patch Merging Layers  
- Global Average Pooling  
- Fully Connected Classification Head  

---

## 📊 Dataset

**Brain Tumor MRI Dataset (Kaggle)**

Classes:
- Glioma  
- Meningioma  
- No Tumor  
- Pituitary  

---

## 📈 Results

---

## 📊 Classification Report

### 📌 Overall Performance

- **Accuracy:** 93%
- **Macro Avg F1-score:** 0.93
- **Weighted Avg F1-score:** 0.93

---

### 🧾 Class-wise Performance

| Class        | Precision | Recall | F1-score | Support |
|--------------|----------|--------|----------|---------|
| Glioma       | 0.99     | 0.77   | 0.87     | 400     |
| Meningioma   | 0.89     | 0.96   | 0.92     | 400     |
| No Tumor     | 0.92     | 1.00   | 0.96     | 400     |
| Pituitary    | 0.96     | 1.00   | 0.98     | 400     |

---

### 📌 Key Insights

- 🧠 Glioma shows **high precision but lower recall**, meaning few false positives but some missed cases  
- 🧠 Meningioma performs well with balanced precision and recall  
- 🧠 No Tumor and Pituitary classes show **near-perfect recall (1.00)**  
- 🎯 Overall model demonstrates strong generalization across all classes  

---

---

## ⚙️ Tech Stack

- Python 🐍  
- PyTorch 🔥  
- NumPy  
- Matplotlib  
- Scikit-learn  
- Seaborn  
- PIL  
- Torchvision  
- KaggleHub  

---

## 🏋️ Training Details

- Image size: 224 × 224  
- Batch size: 16  
- Optimizer: AdamW  
- LR Scheduler: CosineAnnealingWarmRestarts  
- Epochs: 100  
- Loss Function: CrossEntropyLoss  
- Mixed Precision Training: Enabled (AMP)  

---


---

## 🧪 Key Observations

- Swin Transformer effectively captures spatial dependencies in MRI scans  
- Shifted window mechanism improves cross-region feature learning  
- Patch merging enables hierarchical representation  
- Model performs best on structurally distinct classes (e.g., No Tumor)  

---

## 📜 Citation

If you use this project, please cite:

> Swin Transformer-based Brain Tumor Classification (Custom Implementation)

---

## ✨ Author

**Hasib Ur Rahman**  
B.Sc. Software Engineering  
Daffodil International University
