
# 🌸 Ovarytales:Decoding the silent signs of PCOS with data, science, and care.

_"In every cycle lies a story, in every feature a whisper.  
Through data we listen, through models we see clearer."_  

---

## 📖 Overview

**Ovarytales** is a data-driven project aimed at detecting and understanding **Polycystic Ovary Syndrome (PCOS)** using advanced machine learning techniques. From cleaning messy clinical data to visualizing the hidden signals of hormonal imbalance, this project takes you on a journey through symptom patterns, statistical truths, and powerful models — all with a focus on *interpretable AI for healthcare*.

---

## 🔬 Project Flow

### 🧹 1. Data Cleaning & Preprocessing
- Converted string-based numerics into proper numerical form
- Stripped column names, renamed for ease
- Replaced missing values with **median** (robust to outliers)
- Log-transformed skewed features and removed redundant ones (e.g., BMI, Follicle R)

### 📊 2. Exploratory Data Analysis
- Correlation heatmaps to identify significant features
- Violin plots for distribution insights grouped by PCOS status
- Bar charts to explore symptom frequency and lifestyle indicators

### 🔎 3. Feature Engineering
- Discretized cycle length
- Combined hormone ratios (e.g., FSH/LH)
- Selected top features based on Extra Trees importance

---

## 🧠 Models Applied

| Model | Highlights | Recall (PCOS) | Accuracy |
|-------|-----------|---------------|----------|
| 🌲 Random Forest | Baseline, interpretable | 64% | 87% |
| 🔮 Neural Network | Tuned with KerasTuner | 72% | 86% |
| ⚙️ SVM + ADASYN | Perfect recall, best F1 | **100%** | **97.8%** |
| 🧩 Explainable Boosting Machine | Interpretable + Powerful | 96% | 95.6% |

---

## 💡 Key Takeaways

- **Follicle count** and **cycle irregularity** emerged as dominant predictors
- **SVM** excelled in performance, while **EBM** stood out for interpretability
- Lifestyle features had limited impact; biological indicators were stronger
- Feature selection + class balancing drastically improved detection

---

## 👥 Team

This project is crafted with care by:
- **Nandhika Rajmanikandan**
- **Kavya Sri Pachchava** 

---

## 🧭 Purpose

To empower healthcare systems with **accurate**, **ethical**, and **interpretable** AI tools for early PCOS detection — helping women receive the care they deserve, faster.

---

## 📂 Project Structure (Simplified)
```bash
├── data/               # Raw and cleaned datasets
├── notebooks/          # EDA, model training, visualizations
├── models/             # Trained models (optional)
├── utils/              # Helper functions
├── README.md           # Project overview
