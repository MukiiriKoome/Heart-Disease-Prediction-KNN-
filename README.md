# Heart Disease Prediction using K-Nearest Neighbors (KNN)

A machine learning project that predicts the likelihood of heart disease in patients using the **K-Nearest Neighbors (KNN)** algorithm.

## Overview

Cardiovascular disease is one of the leading causes of death worldwide. This project builds a classification model that uses patient clinical data to predict the presence of heart disease, aiming to support early detection and diagnosis.

## Dataset

- **Name:** Heart Failure Prediction Dataset
- **Source:** [Kaggle — fedesoriano](https://www.kaggle.com/datasets/fedesoriano/heart-failure-prediction)
- **Description:** Combines five heart datasets into one, with 11 clinical features (e.g. age, sex, chest pain type, resting blood pressure, cholesterol, fasting blood sugar, max heart rate, exercise-induced angina) and a binary target indicating heart disease presence.

## Approach

1. **Data Loading & Cleaning** — Import the dataset, handle missing/invalid values, check data types.
2. **Exploratory Data Analysis (EDA)** — Visualize feature distributions and relationships with the target variable.
3. **Preprocessing** — Encode categorical variables, scale numerical features (crucial for KNN since it's distance-based).
4. **Train/Test Split** — Partition the data for unbiased evaluation.
5. **Model Building** — Train a KNN classifier.
6. **Hyperparameter Tuning** — Use `GridSearchCV` / cross-validation to find the optimal value of `k`.
7. **Evaluation** — Assess performance using accuracy, precision, recall, F1-score, and a confusion matrix.

## Tech Stack

- Python
- Jupyter Notebook
- pandas, NumPy
- scikit-learn
- Matplotlib / Seaborn

## Results

| Metric | Score |
|---|---|
| Accuracy | *TBD* |
| Precision | *TBD* |
| Recall | *TBD* |
| F1-Score | *TBD* |

*(Fill in with your actual results after running the notebook.)*

## Getting Started

### Prerequisites
```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```

### Run the notebook
```bash
git clone <your-repo-url>
cd heart-disease-knn
jupyter notebook heart_disease_knn.ipynb
```

## Project Structure
```
heart-disease-knn/
├── data/
│   └── heart.csv
├── heart_disease_knn.ipynb
├── README.md
└── requirements.txt
```

## Why KNN?

KNN is a simple, intuitive, non-parametric algorithm well-suited for this classification task — it classifies a new patient based on the majority class among their "k" most similar patients in the training data, based on clinical feature similarity.

## License

This project is open source and available under the [MIT License](LICENSE).

## Acknowledgments

- Dataset by [fedesoriano](https://www.kaggle.com/fedesoriano) on Kaggle.
