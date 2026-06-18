# ❤️ Heart Disease Prediction — Classification Analysis

> A machine learning project that predicts the presence of heart disease using three classification models: Logistic Regression, Decision Tree, and Random Forest. Models are evaluated and compared using accuracy, precision, recall, and F1 score.

---

## 📌 Project Overview

This project applies supervised machine learning to a heart disease dataset to build a binary classifier that predicts whether a patient has heart disease (`1`) or not (`0`). Three models are trained, evaluated, and compared side by side using standard classification metrics and confusion matrices.

---

## 📁 Repository Structure

```
├── fixed.ipynb          # Main Jupyter Notebook (all code & analysis)
├── heartt.csv           # Dataset (2000 patient records, 14 features)
├── requirements.txt     # Python dependencies
└── README.md            # Project documentation
```

---

## 📊 Dataset

| Property | Value |
|---|---|
| Samples | 2000 rows |
| Features | 13 input features + 1 target |
| Target | `0` = No Heart Disease, `1` = Heart Disease |

**Features:**
`age`, `sex`, `cp` (chest pain type), `trestbps` (resting blood pressure), `chol` (cholesterol), `fbs` (fasting blood sugar), `restecg`, `thalach` (max heart rate), `exang` (exercise-induced angina), `oldpeak`, `slope`, `ca`, `thal`

---

## 🧠 Models Used

| Model | Library |
|---|---|
| Logistic Regression | `sklearn.linear_model` |
| Decision Tree | `sklearn.tree` |
| Random Forest | `sklearn.ensemble` |

All models are trained on an 80/20 train-test split with stratification. Features are standardized using `StandardScaler` before training.

---

## 📈 Notebook Sections

| # | Section |
|---|---|
| 1 | Import Libraries |
| 2 | Load & Explore Data |
| 3 | Check Missing Values & Statistics |
| 4 | Target Variable Distribution |
| 5 | Train-Test Split & Feature Scaling |
| 6 | Logistic Regression — Train & Evaluate |
| 7 | Sample Prediction (single patient input) |
| 8 | Visualization: Target Distribution |
| 9 | Confusion Matrix: Logistic Regression |
| 10 | Decision Tree & Random Forest Training |
| 11 | Confusion Matrices: All 3 Models |
| 12 | Precision, Recall & F1 Score Comparison |

---

## ⚙️ Installation & Usage

### 1. Clone the repository
```bash
git clone https://github.com/rifaro7/heart-disease-prediction.git
cd heart-disease-prediction
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Launch the notebook
```bash
jupyter notebook fixed.ipynb
```

Run all cells from top to bottom (`Kernel → Restart & Run All`).

---

## 📦 Requirements

- Python 3.8+
- pandas, numpy
- matplotlib, seaborn
- scikit-learn
- jupyter

See `requirements.txt` for pinned versions.

---

## 📉 Key Visualizations

- **Target Distribution** bar chart (Disease vs No Disease)
- **Confusion Matrices** for all 3 models
- **Precision, Recall & F1 Score** comparison across models

---

## 🔍 Key Findings

- Logistic Regression provides a strong baseline with good generalization
- Random Forest typically achieves the highest accuracy on this dataset
- Stratified splitting ensures balanced class representation in train/test sets
- StandardScaler improves Logistic Regression performance significantly

---

## 👤 Author

Rifa Tasnim Roza

Institution: East West University

---

## 📄 License

This project is for academic purposes. Dataset is used for educational analysis only.
