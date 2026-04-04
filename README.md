# Student Performance Analysis and Prediction

**Student ID: bitsom_ba_25111052**

## Introduction

This project focuses on analyzing student academic performance and building a machine learning model to predict whether a student will pass or fail. The dataset contains information on student scores across multiple subjects, attendance percentage, and daily study hours. The objective is to understand patterns in student performance and apply data-driven techniques to make predictions.

## Dataset Description

The dataset consists of 15 student records with the following columns:

* name: Student name
* math: Math score
* science: Science score
* english: English score
* history: History score
* pe: Physical Education score
* attendance_pct: Attendance percentage
* study_hours_per_day: Average study hours per day
* passed: Target variable (1 = Pass, 0 = Fail)

Given the small size of the dataset, the focus of this project is on understanding the workflow rather than achieving high model accuracy.

## Task 1: Data Exploration

The dataset was loaded using pandas and explored using standard data analysis techniques. The following steps were performed:

* Displayed the first few rows to understand the structure of the dataset
* Checked dataset dimensions and data types
* Generated summary statistics such as mean, minimum, maximum, and standard deviation
* Counted the number of students who passed and failed
* Calculated average subject scores separately for passing and failing students
* Identified the student with the highest overall average score

## Task 2: Data Visualization using Matplotlib

Several visualizations were created using Matplotlib:

* Bar chart showing average scores for each subject
* Histogram displaying the distribution of math scores
* Scatter plot comparing study hours per day with average score, separated by pass/fail
* Box plot comparing attendance percentages between passing and failing students
* Line plot showing math and science scores across all students

## Task 3: Data Visualization using Seaborn

Seaborn was used for statistical visualizations:

* Bar plots comparing average math and science scores for passing and failing students
* Scatter plot of attendance percentage versus average score with regression lines

Seaborn simplifies visualization creation and produces more aesthetically consistent plots compared to Matplotlib.

## Task 4: Machine Learning Model

A Logistic Regression model was implemented to predict whether a student will pass or fail.

### Data Preparation

* Selected relevant features excluding the student name
* Split the dataset into training and testing sets (80:20 ratio)
* Standardized the feature values using StandardScaler

### Model Training

* Trained the Logistic Regression model on the training data
* Evaluated training accuracy

### Model Evaluation

* Generated predictions on the test dataset
* Calculated test accuracy
* Compared predicted and actual values for each student

Due to the small dataset size, accuracy may vary and should be interpreted cautiously.

### Feature Importance

Model coefficients were analyzed to determine the influence of each feature. Positive coefficients indicate a higher likelihood of passing, while negative coefficients suggest a higher likelihood of failing.

### New Student Prediction

A sample student input was used to demonstrate prediction and probability estimation using the trained model.

## Observations

* Higher study hours and attendance are generally associated with better performance
* Students with consistently high subject scores are more likely to pass
* Attendance plays an important role in overall academic success

## Conclusion

This project demonstrates a complete workflow of data analysis and machine learning, including data exploration, visualization, and predictive modeling. The primary goal is to understand the process rather than achieve high predictive accuracy.

## Files Included

* part4_visualization_ml.ipynb
* students.csv

## Notes

* All visualizations are included within the notebook
* The notebook is fully executable from start to finish
