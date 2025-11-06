# 🧠 Breast Cancer Classification (scikit-learn)

This project demonstrates a **supervised machine learning classification** workflow using the **Breast Cancer Wisconsin dataset** from scikit-learn.  
It compares three models — **Logistic Regression**, **Random Forest**, and a **Multi-Layer Perceptron (MLP)** — to predict whether a tumor is *malignant* or *benign*.  
The goal is to explore model performance across various evaluation metrics and visualize the results using ROC curves and a confusion matrix.

---

##  Dataset
- **Source:** `sklearn.datasets.load_breast_cancer`
- **Samples:** 569
- **Features:** 30 numeric attributes describing cell nuclei
- **Target:**  
  - 0 → Malignant  
  - 1 → Benign

---

## Models Implemented
| Model | Description | Scaling Used |
|--------|--------------|--------------|
| Logistic Regression | Linear baseline classifier | ✅ Yes |
| Random Forest | Ensemble of decision trees | ❌ No |
| MLPClassifier | Small neural network with one hidden layer | ✅ Yes |

Each model was trained using a **pipeline** to maintain consistent preprocessing and avoid data leakage.

---

## Evaluation Metrics
All models were evaluated on:
- **Accuracy**
- **Precision**
- **Recall**
- **F1 Score**
- **ROC-AUC**

The **Logistic Regression model** achieved the best overall performance with a ROC-AUC ≈ **0.99**.

---

## Visualizations
The notebook includes:
- **ROC Curves** comparing all three models  
- **Confusion Matrix** for the best-performing model 
