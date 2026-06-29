# 🧠 Brain Tumor Classification using Machine Learning

> Predicting whether a brain tumor is **Benign or Malignant** using clinical patient data and a Random Forest Classifier.

---

## 📌 Project Overview

Brain tumor diagnosis is a critical and time-sensitive medical challenge. This project applies Machine Learning to classify brain tumors based on clinical features such as tumor size, stage, histology type, and patient history.

This is an **educational research project** built as part of my coursework in Artificial Intelligence & Machine Learning.

> ⚠️ **Medical Disclaimer:** This tool is for research and educational purposes only. It is **not** a substitute for professional medical diagnosis. Always consult a qualified doctor.

---

## 🎯 Objective

- Binary classification: **Benign vs Malignant**
- Build a clean, leakage-free ML pipeline
- Provide an interactive patient prediction form

---

## 📊 Dataset

- **Source:** [Brain Tumor Dataset – Kaggle](https://www.kaggle.com/)
- **Features include:** Age, Tumor Size, Stage, Histology, Location, MRI Result, Treatment History, Symptoms, and more
- **Target column:** `Tumor_Type` (Benign / Malignant)

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3 | Core language |
| Pandas & NumPy | Data manipulation |
| Scikit-learn | ML model & evaluation |
| Matplotlib & Seaborn | Visualizations |
| Google Colab | Development environment |

---

## ⚙️ ML Pipeline

```
Raw Data
   ↓
Data Cleaning (duplicates, missing values)
   ↓
Feature Engineering (encoding, scaling)
   ↓
Train / Test Split (80/20, stratified)
   ↓
Random Forest Classifier
   ↓
Evaluation (Accuracy, AUC-ROC, Cross-Validation)
   ↓
Live Patient Prediction
```

---

## 📈 Model Performance

| Metric | Score |
|--------|-------|
| Test Accuracy | ~XX% *(run notebook to see)* |
| 5-Fold CV Mean | ~XX% |
| AUC-ROC | ~X.XX |

> Results depend on the dataset version used. No accuracy was hardcoded — all numbers are genuine model outputs.

---

## 🔍 Key Features of This Project

- ✅ **No data leakage** — features are only derived from original dataset columns
- ✅ **Real model confidence** — probabilities come directly from `predict_proba()`
- ✅ **Balanced classes** — `class_weight='balanced'` handles imbalanced data
- ✅ **Interactive prediction** — Colab sliders let you test any patient profile
- ✅ **Feature importance plot** — shows which clinical features matter most

---

## 📁 Project Structure

```
brain-tumor-classification/
│
├── brain_tumor_fixed.ipynb   # Main notebook (clean pipeline)
├── brain_tumor_dataset.csv   # Dataset (download from Kaggle)
├── model_analysis.png        # Confusion matrix + feature importance
├── correlation_heatmap.png   # Feature correlation heatmap
└── README.md                 # This file
```

---

## 🚀 How to Run

1. Open `brain_tumor_fixed.ipynb` in [Google Colab](https://colab.research.google.com/)
2. Upload `brain_tumor_dataset.csv` when prompted
3. Run all cells in order (Runtime → Run All)
4. In **Cell 7**, adjust the sliders to test different patient profiles

---

## 📸 Sample Output

```
=======================================================
🧠 BRAIN TUMOR CLASSIFICATION REPORT
=======================================================
📋 Patient  : Age 45 | Female
🔬 Tumor    : Meningioma | Frontal lobe | Stage II | Size 3.2 cm
-------------------------------------------------------
📊 Model Probabilities (from Random Forest):
   Benign      : 78.40%  ████████████████████████
   Malignant   : 21.60%  ██████
-------------------------------------------------------
🤖 Prediction : Benign
📈 Confidence : 78.40%  (actual model output — not hardcoded)
-------------------------------------------------------
✅ Low Risk — Routine monitoring and follow-up advised.

⚠️  DISCLAIMER: ML research tool only. NOT a medical diagnosis.
=======================================================
```

---

## 👩‍💻 About

**Developed by:** Ayesha Farooq  
**University:** University of Narowal  
**Program:** BS Computer Science — Semester 6  
**Focus Area:** Artificial Intelligence & Machine Learning

---

## 📬 Contact

Feel free to connect or give feedback:

- GitHub: [@ayesha-cs-93](https://github.com/ayesha-cs-93)
- Email: ayesha.farooq.cs93@gmail.com

---

*If you found this project helpful, please ⭐ star the repository!*
