## Credit Card Fraud Detection

This project implements fraud detection on credit card transactions using multiple machine learning models, advanced data visualization, and evaluation metrics. It uses the Kaggle Credit Card Fraud Dataset, which contains anonymized transaction data labeled as fraudulent (Class = 1) or legitimate (Class = 0).

Fraud detection is a critical application of machine learning in the financial sector, helping prevent unauthorized transactions and minimize financial losses.



## 📌 Features

## Exploratory Data Analysis (EDA)

Visualization of class imbalance between legitimate and fraudulent transactions.

Analysis of transaction patterns by time and amount.

Generation of correlation heatmaps and feature distribution plots to understand relationships in the dataset.


## Machine Learning Models Implemented

Random Forest – Ensemble-based decision trees for robust predictions.

AdaBoost – Boosting technique to improve weak learners.

CatBoost – Gradient boosting on categorical features with high performance.

XGBoost – Popular boosting algorithm optimized for speed and accuracy.

LightGBM – Gradient boosting model optimized for large datasets and fast training.


## Evaluation Metrics

Confusion Matrix – Provides true positives, false positives, true negatives, and false negatives.

ROC-AUC Score – Measures the ability of the model to distinguish between fraudulent and legitimate transactions.

Feature Importance – Identifies the most significant features contributing to fraud prediction.





## 📂 Project Structure
credit_card_fraud_detection.py   # Main Python script for training and evaluation
creditcard.csv                   # Dataset (download separately from Kaggle)
README.md                        # Project documentation




## 🗂 Dataset

Source: Kaggle Credit Card Fraud Detection Dataset

Description: The dataset contains 284,807 credit card transactions made by European cardholders in September 2013.

Class Distribution:

Legitimate transactions (Class = 0): 284,315

Fraudulent transactions (Class = 1): 492

Features:

Time – Seconds elapsed between this transaction and the first transaction in the dataset.

V1–V28 – Principal components obtained via PCA to protect sensitive information.

Amount – Transaction amount.

Class – Target variable (0 = legitimate, 1 = fraud).




## ⚙️ Requirements

Before running the project, install the required dependencies:

pip install pandas numpy matplotlib seaborn plotly scikit-learn xgboost lightgbm catboost





## ▶️ How to Run

Download the dataset creditcard.csv from Kaggle and place it in your working directory (or update the file path in the script).

Run the script:

python credit_card_fraud_detection.py


The script will:

Load and preprocess the dataset.

Perform exploratory data analysis (EDA).

Train multiple machine learning models.

Display visualizations of data and model performance.

Output confusion matrices, ROC-AUC scores, and feature importance.



## 📊 Results

Credit card fraud detection is a highly imbalanced classification problem, with very few fraudulent transactions compared to legitimate ones.

Models like XGBoost and LightGBM generally perform better due to their handling of class imbalance and boosting techniques.

Evaluation metrics help assess performance:

Confusion Matrix: Accuracy of fraud detection.

ROC-AUC Score: Ability to distinguish between classes.

Feature Importance: Insights into which features contribute most to predictions.



## 🚀 Future Improvements

Implement SMOTE or undersampling to handle data imbalance.

Deploy the trained model as an API using Flask or FastAPI.

Perform hyperparameter tuning for boosting models to improve accuracy.

Integrate real-time fraud detection with streaming transaction data.
