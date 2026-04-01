Student Performance Analysis & Prediction
Overview

This project analyses student performance data, produces visualizations, and builds a machine learning model to predict whether a student will pass or fail based on multiple features such as scores, attendance, and study hours.

The project is divided into 4 main tasks:

Data Exploration with Pandas
Matplotlib Visualizations
Seaborn Visualizations
Machine Learning with scikit-learn
Dataset

The dataset (students.csv) contains 15 students with the following columns:

Column	Description
name	Student name
math	Math score
science	Science score
english	English score
history	History score
pe	Physical Education score
attendance_pct	Attendance percentage
study_hours_per_day	Daily study hours
passed	Target: 1 = Pass, 0 = Fail
Task Summary
1. Data Exploration
Loaded data using pandas.read_csv().
Displayed first 5 rows, shape, column types, and summary statistics.
Counted the number of passing and failing students.
Calculated average scores per subject for Pass and Fail groups.
Identified the student with the highest overall average.
2. Matplotlib Visualizations

Saved as PNG files:

plot1_bar.png: Average score per subject (Bar Chart)
plot2_hist.png: Math scores distribution (Histogram)
plot3_scatter.png: Study hours vs average score (Scatter Plot)
plot4_box.png: Attendance distribution for Pass vs Fail (Box Plot)
plot5_line.png: Math and Science scores per student (Line Plot)
3. Seaborn Visualizations

Saved as PNG files:

plot6_seaborn_bar.png: Average Math & Science scores by Pass/Fail (Bar Plot)
plot7_seaborn_scatter.png: Attendance vs average score with regression lines (Scatter Plot)

Observation: Seaborn made it easier to add regression lines and color-coded plots, while Matplotlib provided more control for customized charts.

4. Machine Learning
Features: math, science, english, history, pe, attendance_pct, study_hours_per_day
Target: passed
Split into train (80%) and test (20%), scaled features with StandardScaler.
Trained LogisticRegression classifier.
Evaluated test accuracy and compared predictions with actual labels.
Generated feature importance chart (feature_importance.png) highlighting which features contribute positively or negatively towards passing.
Bonus: Predicted pass/fail for a new student and displayed probabilities.
