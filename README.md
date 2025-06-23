# Credit-card-fraud-detection-using-Logistic-Regression

This project demonstrates fraud detection on credit card transactions using Logistic Regression in Python. The process includes data loading, preprocessing (including concatenating two datasets due to the lack of sufficient fraud samples), model training, and evaluation—all within a Jupyter notebook.

Dataset
Two credit card transaction datasets were concatenated to address the scarcity of fraudulent transactions, ensuring a more balanced and realistic dataset for model training.
The resulting dataset contains anonymized features (V1 to V28), transaction Amount, and a target column Class (1: Fraud, 0: Not Fraud).
Steps Performed
Import Libraries

numpy, pandas, scikit-learn modules for data handling and modeling.
Load and Combine Data

Both datasets are loaded using pandas.
They are concatenated to create a single, larger DataFrame with more fraud cases.
Initial Exploration

Display the first few rows and check for null values.
Analyze class distribution to observe class imbalance.
Data Cleaning

Drop the id column as it is not relevant for prediction.
Feature Selection

Features: All columns except Class.
Target: Class.
Train-Test Split

Split the dataset into training and testing sets.
Model Training

Train a Logistic Regression model.
Evaluation

Predict on the test set and compute accuracy.

Requirements
Python 3.x
numpy
pandas
scikit-learn
Jupyter notebook or Google Colab
Install dependencies with:

sh
pip install numpy pandas scikit-learn
Notes
The concatenation of two datasets was necessary due to the rarity of fraud samples, helping the model learn more effectively.
The dataset remains highly imbalanced; consider using additional metrics (precision, recall, F1-score) for better evaluation.
Further improvements could include data balancing, feature engineering, or trying advanced algorithms.
