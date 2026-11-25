# Heart Disease Classification Using Machine Learning

## Project Overview
This project explores supervised machine learning techniques for binary classification of heart disease. The objective is to predict the presence or absence of heart disease based on clinical and demographic features and compare the performance of different classification algorithms.

## Dataset
- **File:** `heart.csv`
- **Initial records:** 303
- **Features:** 13 input features
- **Target variable:** `output`
- **Task:** Binary classification
- **Missing values:** None
- **Duplicate records:** 1 removed

The dataset includes features such as age, sex, chest pain type, resting blood pressure, cholesterol, maximum heart rate, and other clinical measurements.

## Methodology
1. Data inspection and descriptive statistical analysis
2. Exploratory Data Analysis (EDA) and feature distribution visualization
3. Correlation analysis
4. Duplicate removal and data preparation
5. Stratified train-test split (80/20)
6. Feature scaling using StandardScaler
7. Model training and performance evaluation

## Machine Learning Models
The following classification algorithms were implemented and compared:

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Decision Tree
- Support Vector Machine (SVM with RBF kernel)

## Model Evaluation

The models were evaluated using Accuracy, Precision, Recall, F1-score, and Confusion Matrix.

| Model | Accuracy |
|---|---:|
| Logistic Regression | 78.69% |
| KNN | 80.33% |
| Decision Tree | 72.13% |
| SVM | **83.61%** |

SVM achieved the highest accuracy among the evaluated models on the held-out test split.

## Additional Experiment: Hyperparameter Tuning
A separate SVM hyperparameter tuning experiment was conducted using GridSearchCV on the Iris dataset with 5-fold cross-validation.

- Best parameters: `C=1`, `gamma=0.01`, `kernel=linear`
- Best cross-validation accuracy: 98%

This experiment is separate from the heart disease classification task.

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Repository Structure
```text
heart-disease-classification/
│
├── classification.ipynb
├── heart.csv
└── README.md
```

## How to Run
1. Clone this repository.
2. Install the required Python libraries.
3. Ensure `heart.csv` is in the same directory as the notebook.
4. Open and run `classification.ipynb` using Jupyter Notebook or Google Colab.

## Disclaimer
This project is an educational machine learning exercise and is not intended for clinical diagnosis or medical decision-making.
