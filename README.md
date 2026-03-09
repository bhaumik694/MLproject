🎯 Math Score Predictor
Machine Learning Project for Predicting Student Academic Performance

📌 Overview

The Math Score Predictor is a machine learning project that predicts a student's math exam score based on demographic and academic factors.
The project explores how different variables such as gender, parental education, lunch type, and test preparation influence student performance.
Multiple regression models are trained and evaluated to determine the best predictive model.

🧠 Problem Statement

Educational institutions often analyze factors that affect student performance to improve academic outcomes.
This project aims to predict math scores using machine learning by analyzing the following features:

Gender
Race / Ethnicity
Parental level of education
Lunch type
Test preparation course
Reading score
Writing score

The trained model can be used to estimate math performance based on these factors.

📊 Dataset

Source:
🔗 https://www.kaggle.com/datasets/spscientist/students-performance-in-exams?datasetId=74977

Dataset Characteristics
Attribute	Value
Number of Rows	1000
Number of Columns	8
Problem Type	Regression
Dataset Features
Feature	Description
gender	Student gender
race_ethnicity	Ethnicity group
parental_level_of_education	Parent's highest education level
lunch	Type of lunch (standard / free)
test_preparation_course	Course completion status
reading_score	Reading exam score
writing_score	Writing exam score
math_score	Target variable
⚙️ Machine Learning Pipeline

The project follows a structured ML pipeline:

Data Collection
      ↓
Data Preprocessing
      ↓
Feature Engineering
      ↓
Model Training
      ↓
Model Evaluation
      ↓
Best Model Selection

🤖 Machine Learning Models Used

The following regression algorithms were trained and evaluated:

Model	Description
Linear Regression	Baseline regression model
Ridge Regression	L2 regularized regression
Lasso Regression	L1 regularized regression
KNN Regressor	Distance-based regression
Decision Tree Regressor	Tree-based model
Random Forest Regressor	Ensemble tree model
AdaBoost Regressor	Boosting algorithm
XGBoost Regressor	Gradient boosting model
CatBoost Regressor	Optimized gradient boosting
📈 Model Evaluation Metrics

Models were evaluated using:

MAE — Mean Absolute Error
RMSE — Root Mean Squared Error
R² Score — Coefficient of determination

Example evaluation function:

def evaluate_model(true, predicted):
    mae = mean_absolute_error(true, predicted)
    mse = mean_squared_error(true, predicted)
    rmse = np.sqrt(mean_squared_error(true, predicted))
    r2_square = r2_score(true, predicted)
    return mae, rmse, r2_square


🛠 Tech Stack
Programming Language
Python
Libraries
Pandas
NumPy
Matplotlib
Seaborn
Scikit-Learn
XGBoost
CatBoost

📁 Project Structure
Math-Score-Predictor
│
├── data/
│   └── stud.csv
│
├── notebooks/
│   └── MODEL_TRAINING.ipynb
│
├── src/
│   └── training_pipeline.py
│
├── requirements.txt
│
└── README.md

🚀 How to Run the Project

1️⃣ Clone the repository
git clone https://github.com/yourusername/math-score-predictor.git

2️⃣ Install dependencies
pip install -r requirements.txt

3️⃣ Run the notebook
jupyter notebook

Open:
MODEL_TRAINING.ipynb
