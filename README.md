# Task32
Student Performance & Learning Analytics

1. Project Overview

This project analyzes student academic and learning data to identify performance patterns, subject-wise strengths and weaknesses, attendance trends, and factors associated with successful outcomes.

2. Objectives

- Analyze student academic performance.
- Identify subject-wise strengths and weaknesses.
- Analyze attendance trends.
- Perform data cleaning.
- Create data visualizations.
- Perform statistical analysis.
- Introduce predictive modeling.

3. Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
- Excel
- Git & GitHub

4. Project Workflow

1. Data Collection
2. Data Cleaning
3. Exploratory Data Analysis (EDA)
4. Data Visualization
5. Statistical Analysis
6. Predictive Modeling

5. Python Code

Step 1: Import Libraries

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

Step 2: Load Dataset

df = pd.read_csv("student_data.csv")
print(df.head())

Step 3: Explore Dataset

print(df.shape)
print(df.info())
print(df.describe())

Step 4: Check Missing Values

print(df.isnull().sum())

Step 5: Remove Duplicate Rows

df = df.drop_duplicates()
print(df)

Step 6: Data Visualization

df.select_dtypes(include="number").hist(figsize=(10, 8))
plt.tight_layout()
plt.show()

Step 7: Correlation Analysis

sns.heatmap(df.select_dtypes(include="number").corr(),
            annot=True, cmap="coolwarm")
plt.show()

6. Expected Outcomes

- Understand student performance patterns.
- Identify academic strengths and weaknesses.
- Understand attendance trends.
- Visualize student academic data.
- Learn basic predictive modeling.

7. Deliverables

- Student Dataset
- Cleaned Dataset
- Python Code
- Data Visualizations
- Statistical Analysis
- Predictive Modeling

8. Conclusion

This project helps analyze student academic performance using Data Science techniques. It provides practical experience in Python programming, data cleaning, visualization, and statistical analysis.

9. Author

Data Science Intern – VEDA Technology
