# Classification-model
Project Overview

This project focuses on predicting whether a passenger survived the Titanic disaster using Machine Learning classification algorithms. The project uses passenger information to train and evaluate predictive models.

Dataset

The project uses the Titanic dataset, which contains passenger information.
Target Variable: Survived

0: Did not survive

1: Survived

Tools & Libraries

Python

Pandas

Scikit-learn

Google Colab


1. Data Loading

Loaded the Titanic dataset using Pandas.

2. Feature Engineering

Created three new features to improve the model's ability to identify patterns:

Title: Extracted passenger titles from their names.

FamilySize: Calculated the total number of family members aboard.

IsAlone: Identified whether a passenger was traveling alone.

3. Train-Validation Split

Split the dataset into training and validation sets using train_test_split.

4. Data Preprocessing

Applied preprocessing techniques using Scikit-learn:

Missing Values: Used median imputation for numerical features and most frequent imputation for categorical features.

Encoding: Applied OneHotEncoder to convert categorical features into numerical representations.

ColumnTransformer: Applied different preprocessing steps to numerical and categorical columns.

5. Model Training

Trained and evaluated two classification algorithms:

Logistic Regression: Used as the first classification model.

Random Forest Classifier: Used as the second classification model.

6. Hyperparameter Tuning

Used GridSearchCV with 5-fold cross-validation to find the best Random Forest hyperparameters.

The parameters included:

n_estimators

max_depth

min_samples_split

max_features

7. Model Evaluation

Evaluated the models using the following metrics:

Accuracy Score

Confusion Matrix

Classification Report (Precision, Recall, and F1-score)

