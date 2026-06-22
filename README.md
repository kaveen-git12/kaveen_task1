# Kaveen_Task1 — Iris Flower Classification

**Oasis Infobyte Data Science Internship — Task 1**

## 📌 Objective
Train a machine learning classification model to identify the species of an iris flower
(*Setosa*, *Versicolor*, or *Virginica*) from its physical measurements: sepal length,
sepal width, petal length, and petal width.

## 🛠️ Tech Stack
- Python 3
- pandas, numpy
- scikit-learn
- matplotlib, seaborn
- Jupyter Notebook

## 📂 Files
| File | Description |
|---|---|
| `Kaveen_Task1.ipynb` | Complete, pre-executed Jupyter notebook with all code, outputs, and visualizations |

## 📊 Dataset
The classic **Iris dataset** (150 samples, 3 classes, 50 samples per class), loaded directly
from `sklearn.datasets.load_iris()` — no external download required.

## 🔍 Workflow
1. **Data loading** — via scikit-learn's built-in dataset
2. **Exploratory Data Analysis (EDA)** — shape, dtypes, null check, descriptive statistics (overall and per species)
3. **Visualizations** — pairplot/scatter matrix by species, box plots per feature, correlation heatmap
4. **Feature selection discussion** — identifying petal length and petal width as the most discriminative features
5. **Train/test split** — 80/20 stratified split
6. **Model training** — four classifiers trained and compared:
   - Logistic Regression
   - K-Nearest Neighbours (KNN)
   - Decision Tree
   - Random Forest
7. **Model evaluation** — accuracy score, confusion matrix, and full classification report (precision, recall, F1-score) for each model
8. **Best model selection** — comparison table and reasoned justification for the top-performing model

## ✅ Results
All four models achieve high accuracy (90%+) on the held-out test set, since the Iris dataset
is small and the three species are largely (though not perfectly) linearly separable in
petal-length/petal-width space. The only consistent source of misclassification across models
is occasional overlap between *Versicolor* and *Virginica* — *Setosa* is essentially always
classified perfectly. See the notebook for the exact accuracy/precision/recall figures and the
final model recommendation with justification.

## ▶️ How to Run
```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
jupyter notebook Kaveen_Task1.ipynb
```
Run all cells top to bottom — no external data files are needed.

## Acknowledgment
This project was completed as part of the **Data Science Internship** at **Oasis Infobyte**.

---
*Author: Kaveen*
