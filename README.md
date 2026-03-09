##Problem Statement

This project analyzes how a student's performance (test scores) is affected by several factors such as Gender, Ethnicity, Parental level of education, Lunch type, and Test preparation course.
Using these features, the model predicts the math score of a student using machine learning regression algorithms.

Dataset

Source:
https://www.kaggle.com/datasets/spscientist/students-performance-in-exams?datasetId=74977

Dataset details:

Rows: 1000

Columns: 8

##Features in the dataset:

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

##Evaluation Metrics

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

##Visualization

The project includes visualizations such as:

Actual vs Predicted score plots
Regression analysis graphs
These help evaluate how well the model predicts student performance.

##Tech Stack

Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-Learn
XGBoost

CatBoost
