# Predicting Student Performance: A Machine Learning Consultancy Project
## Overview
This project aims to build a machine learning model to predict whether a student will pass or fail the academic year based on various characteristics. We utilized a dataset containing 649 student records with 31 features, including both numerical and categorical data. By applying machine learning techniques, the goal is to identify key factors influencing student performance and create an accurate classification model to predict student outcomes.

## Key Features
Data Preprocessing: We handled various data types (numerical, ordinal, nominal) and employed encoding techniques to prepare the data for machine learning models.

- Feature Selection: Features were selected based on their correlation with the target variable, ‘Pass’ (a binary classification based on whether the grade is above 12).

- Outlier Removal: Outliers were handled using the interquartile range (IQR) method, with specific attention to numerical and ordinal variables.

- Data Scaling: Numerical data was standardized using the StandardScaler function to ensure no bias is introduced during model training.

## Models Used
Three machine learning models were trained and evaluated to predict student performance:

- Random Forest: Chosen for its ability to handle non-linear relationships and overfitting.

- K-Nearest Neighbors (KNN): Simple, adaptable, and non-parametric model.

- Logistic Regression: Specialized for classification problems.

## Model Hyperparameters
- Random Forest: n_estimators, max_depth

- KNN: n_neighbors, p, weights

- Logistic Regression: C, solver

## Model Evaluation
The models were evaluated using:

- Accuracy: The overall percentage of correct predictions.

- Precision: The proportion of positive predictions that were correct.

- Recall: The proportion of actual positives that were correctly identified.

- F1 Score: The harmonic mean of precision and recall.

After tuning the hyperparameters using GridSearch and performing 10-fold cross-validation, the Logistic Regression model was found to provide the best performance with an accuracy of 78.03%, precision of 77.78%, recall of 89.09%, and an F1 score of 83.05%.

## Data Visualizations
Several histograms and box-plots were created to visualize the distribution of numerical features, and a correlation matrix was used to identify relationships between features and the target variable.
