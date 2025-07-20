# ❤️ Heart Disease Prediction

This project analyzes and predicts heart disease using various machine learning models. The dataset is examined for patterns and cleaned through feature selection and multicollinearity reduction. Multiple classifiers are applied to assess predictive performance.

---

## 📂 Dataset

**Source:** `Heart Disease.csv`

Each row in the dataset represents a patient record with features such as age, sex, cholesterol levels, heart rate, and more. The `target` column indicates the presence of heart disease:
- `1` – Patient has heart disease
- `0` – Patient does not have heart disease

---

## 🧪 Exploratory Data Analysis (EDA)

Key steps:
- Checked for missing values and duplicates
- Examined data types and summary statistics
- Visualized:
  - Age distribution by sex
  - Correlation heatmap
  - Count plots by sex and heart disease status
  - Age distribution with swarm, violin, and histogram plots

---

## 🧹 Data Cleaning and Feature Selection

- Removed features with high multicollinearity using Variance Inflation Factor (VIF)
- Dropped `trestbps`, `thalach`, `age`, `chol`, and `thal` iteratively to reduce VIF values
- Final set of independent features stored in `df_ind`

---

## 🤖 Machine Learning Models

### 🔹 Logistic Regression
- Trained on cleaned features
- Evaluated using accuracy, confusion matrix, and classification report

### 🔹 Decision Tree Classifier
- Simple and interpretable model
- Visualized using `plot_tree()`

### 🔹 Random Forest Classifier
- Ensemble method using 50 decision trees
- Generally higher accuracy and robustness

---

## 📈 Evaluation Metrics

Each model is evaluated on:
- **Accuracy Score**
- **Confusion Matrix**
- **Classification Report**: Includes precision, recall, f1-score

---

## 📊 Visualization Examples

- Swarm and violin plots show how age varies across target groups
- Correlation heatmap helps detect multicollinearity
- Tree visualization for interpretability of decision paths

---

## 🛠️ Tech Stack

- Python
- pandas, numpy
- seaborn, matplotlib
- scikit-learn
- statsmodels

---

## 🚀 Getting Started

1. Clone the repo:
```bash
git clone https://github.com/Jay24-coder/Heart_disease.git
cd Heart_disease
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

---

## 🧠 Future Improvements

- Try more advanced models like XGBoost or SVM
- Add hyperparameter tuning (e.g. GridSearchCV)
- Explore feature engineering to enhance model performance

---
