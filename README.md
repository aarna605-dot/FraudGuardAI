# FraudGuardAI

An end-to-end machine learning project for detecting fraudulent credit card transactions. This project compares multiple classification models and evaluates their performance on a highly imbalanced dataset.

## Overview
Credit card fraud detection is a binary classification problem where fraudulent transactions represent less than 0.2% of the data. Since accuracy alone is misleading in such cases, this project focuses on evaluation metrics like Precision, Recall, F1-Score, and ROC-AUC to compare different machine learning models.

## Dataset
The project uses the **Credit Card Fraud Detection** dataset containing **284,807 transactions**, of which **492 are fraudulent**.

- Features `V1`–`V28` are anonymized using PCA.
- `Time` and `Amount` represent transaction metadata.
- `Class` is the target variable:
  - `0` → Genuine transaction
  - `1` → Fraudulent transaction

## Models
- Logistic Regression
- Decision Tree
- Random Forest

## Results

|        Model        |   Accuracy   |   Precision  |    Recall    |   F1 Score   |   ROC-AUC    |
|--------------------:|-------------:|-------------:|-------------:|-------------:|-------------:|
| Logistic Regression |   0.999140   |   0.826667   |   0.632653   |   0.716763   |    0.960549  |
|   Decision Tree     |   0.999368   |    0.897436  |   0.714286   |   0.795455   |    0.830031  |
|  **Random Forest**  | **0.999596** | **0.941176** | **0.816327** | **0.874317** | **0.963027** |

Random Forest achieved the best overall performance and was selected as the final model.

## Visualizations
The notebook includes:

- Class distribution
- Correlation heatmap
- Transaction amount and time distributions
- ROC curves
- Random Forest feature importance

## Tech Stack
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Pickle
- Jupyter Notebook

## Future Improvements
- Hyperparameter tuning
- SMOTE for handling class imbalance
- XGBoost implementation
- Model deployment using Flask or FastAPI

## Author
**Aarna Gupta**

GitHub: https://github.com/aarna605-dot
