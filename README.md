# Task 31 — Features and Target Selection Using Python

## Project Overview

This project demonstrates feature and target selection in a supervised machine-learning problem using Python, Pandas, and Scikit-learn.

A student performance dataset is used to identify suitable input features and a target variable.

The objective is to understand how input variables are selected to predict an output variable in supervised machine learning.

## Objectives

- Understand the structure of a supervised machine-learning problem.
- Explore the student performance dataset.
- Identify numerical and categorical columns.
- Select suitable input features (X).
- Select the target variable (y).
- Explain the reasoning behind feature selection.
- Avoid including the target variable in the input features.
- Demonstrate training and testing data separation.

## Technologies Used

- Python
- Pandas
- Scikit-learn
- Google Colab
- Jupyter Notebook

## Dataset Description

The project uses a manually created student performance dataset containing 20 fictional student records.

The dataset contains seven columns:

| Column | Description |
|---|---|
| student_id | Unique student identifier |
| department | Academic department |
| study_hours | Hours spent studying |
| attendance_pct | Attendance percentage |
| assignment_score | Assignment marks |
| previous_exam_score | Previous examination marks |
| final_exam_score | Final examination marks |

## Selected Input Features (X)

The following four numerical columns are selected as input features:

1. `study_hours`
2. `attendance_pct`
3. `assignment_score`
4. `previous_exam_score`

These variables provide academic information that may help predict examination performance.

## Selected Target Variable (y)

**Target:** `final_exam_score`

This variable represents the final examination score that the supervised machine-learning model is intended to predict.

## Reason for Selection

- Study hours represent the time spent studying.
- Attendance percentage represents student participation.
- Assignment score represents assignment performance.
- Previous examination score represents previous academic performance.
- Final examination score is selected as the prediction target.

The student ID is excluded because it is an identifier rather than a meaningful academic input.

The department column is excluded from this basic numerical feature selection exercise because it requires categorical encoding before use as a numerical model input.

## Feature and Target Shapes

| Component | Shape |
|---|---|
| Input features (X) | (20, 4) |
| Target variable (y) | (20,) |

## Training and Testing Split

The dataset is divided into:

- 80% training data — 16 records.
- 20% testing data — 4 records.

Scikit-learn's `train_test_split()` function is used.

No predictive model is trained in this assignment.

## Project Files

- `Task_31_Features_and_Target_Selection.ipynb` — Complete Colab notebook.
- `student_performance.csv` — Original student dataset.
- `selected_dataset.csv` — Dataset containing selected features and target.
- `X_features.csv` — Selected input feature columns.
- `y_target.csv` — Selected target with student IDs.
- `feature_selection_summary.csv` — Explanation of selected columns.
- `requirements.txt` — Required Python libraries.
- `README.md` — Project documentation.
- `project_report.pdf` — Formal project report.

## Conclusion

This project demonstrates the basic structure of a supervised machine-learning problem by identifying appropriate input features and a target variable.

The selected features provide academic information, while the target represents the final examination score to be predicted.

The exercise provides practical understanding of feature selection, target selection, and training-testing data preparation.
