Problem Statement

This project analyzes how a student's performance (test scores) is affected by several factors such as Gender, Ethnicity, Parental level of education, Lunch type, and Test preparation course.
Using these features, the model predicts the math score of a student using machine learning regression algorithms.

Dataset

Source:
https://www.kaggle.com/datasets/spscientist/students-performance-in-exams?datasetId=74977

Dataset details:

Rows: 1000

Columns: 8

Features in the dataset:

Feature	Description
gender	Gender of the student
race_ethnicity	Ethnicity group
parental_level_of_education	Parent's highest education
lunch	Standard or free lunch
test_preparation_course	Completed or none
reading_score	Reading exam score
writing_score	Writing exam score
math_score	Target variable
Project Workflow

Data Collection

Data Preprocessing

Feature Engineering

Model Training

Model Evaluation

Model Selection

Data Preprocessing
Feature Selection

Target variable:

math_score

Input features:

gender
race_ethnicity
parental_level_of_education
lunch
test_preparation_course
reading_score
writing_score
Encoding

Categorical features are converted using:

OneHotEncoder
Scaling

Numerical features are standardized using:

StandardScaler
Train Test Split

Dataset split:

Training Data: 80%
Testing Data: 20%
Machine Learning Models Used

The following regression models were trained and evaluated:

Linear Regression

Ridge Regression

Lasso Regression

K-Nearest Neighbors Regressor

Decision Tree Regressor

Random Forest Regressor

AdaBoost Regressor

XGBoost Regressor

CatBoost Regressor

Evaluation Metrics

Model performance was evaluated using:

Mean Absolute Error (MAE)

Root Mean Squared Error (RMSE)

R² Score

Example evaluation function:

def evaluate_model(true, predicted):
    mae = mean_absolute_error(true, predicted)
    mse = mean_squared_error(true, predicted)
    rmse = np.sqrt(mean_squared_error(true, predicted))
    r2_square = r2_score(true, predicted)
    return mae, rmse, r2_square
Visualization

The project includes visualizations such as:

Actual vs Predicted score plots

Regression analysis graphs

These help evaluate how well the model predicts student performance.

Tech Stack

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-Learn

XGBoost

CatBoost
