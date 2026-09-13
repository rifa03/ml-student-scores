# Student Performance Prediction Based on Study Hours

## Project Overview

This project analyzes the relationship between study hours and student scores and evaluates regression models to predict student performance.

The analysis focuses on understanding how study hours relate to academic outcomes and comparing multiple regression models to identify the best-performing model for predicting student scores.

The project applies an end-to-end analytical workflow, including data quality checking, exploratory data analysis (EDA), model development, evaluation, and interpretation of results.

---

## Objectives

The objectives of this project are:

- Analyze the relationship between study hours and student scores.
- Perform exploratory data analysis (EDA) to identify patterns in the dataset.
- Build and compare regression models for student score prediction.
- Evaluate model performance using appropriate evaluation metrics.
- Interpret analytical results and identify limitations of the model.

---

## Dataset Description

The dataset contains student study hours and exam scores with the following variables:

| Variable | Role | Description |
|---|---|---|
| Hours | Feature (X) | Number of study hours spent by students |
| Scores | Target (y) | Student exam scores |

Dataset characteristics:

- Total observations: 25 records
- Number of variables: 2 numerical variables
- Analysis type: Regression

The target variable is numerical, therefore regression models are applied to predict student scores based on study hours.

---

## Data Quality Checking

Before modeling, data quality checks were performed to ensure the dataset was suitable for analysis.

The checking process included:

- Missing value identification
- Duplicate data checking
- Data type validation
- Outlier examination using boxplot visualization

Results:

- No missing values were identified.
- No duplicate records were found.
- Both variables were numerical.
- No extreme outliers were detected.

The dataset was considered ready for exploratory analysis and modeling without additional data cleaning steps.

---

## Exploratory Data Analysis

Exploratory Data Analysis (EDA) was conducted to understand the relationship between study hours and student scores.

Key findings:

- Scatter plot analysis shows a positive relationship between study hours and student scores.
- Pearson correlation coefficient between study hours and scores is **0.98**, indicating a very strong linear relationship.
- Students with higher study hours tend to achieve higher scores.

Visualization:

(Add EDA visualization screenshot here)

---

## Methodology

The analytical workflow consists of the following steps:
Dataset
↓
Data Quality Checking
↓
Exploratory Data Analysis
↓
Train-Test Split
↓
Model Training
↓
Prediction
↓
Model Evaluation
↓
Interpretation


Dataset splitting:

- Training data: 75%
- Testing data: 25%
- random_state: 1

The training dataset was used to build the models, while the testing dataset was used to evaluate model performance.

---

## Regression Models

Three regression models were implemented and compared:

### 1. Linear Regression

Linear Regression was used as a baseline model because the dataset shows a strong linear relationship between study hours and student scores.

### 2. Decision Tree Regressor

Decision Tree Regressor was applied to capture more flexible relationships and potential non-linear patterns in the data.

### 3. Random Forest Regressor

Random Forest Regressor combines multiple decision trees to improve prediction stability and generalization performance.

---

## Model Evaluation

Model performance was evaluated using:

### Mean Absolute Error (MAE)

MAE measures the average absolute difference between actual values and predicted values.

### R² Score

R² Score measures how well the model explains the variation in student scores.

| Model | MAE | R² Score |
|---|---:|---:|
| Linear Regression | 7.33 | 0.5860 |
| Decision Tree Regressor | 5.86 | 0.9087 |
| Random Forest Regressor | 5.86 | 0.9023 |

Based on evaluation results, **Decision Tree Regressor achieved the best performance** with the highest R² Score and lowest MAE on the test dataset.

---

## Key Insights

The main findings from this analysis are:

- Study hours have a strong positive relationship with student scores.
- Decision Tree Regressor achieved the best prediction performance among the tested models.
- The best model achieved:
  - MAE: **5.86**
  - R² Score: **0.9087**
- Regression models can predict student scores based on study hours within this dataset.

---

## Limitations

This project has several limitations:

- The dataset contains only **25 observations**, which limits model generalization.
- The model uses only one predictor variable, which is study hours.
- The testing dataset consists of only 7 observations, making evaluation results sensitive to data splitting.
- The analysis identifies correlation between study hours and scores, but it does not prove a causal relationship.

Future improvements:

- Add more student-related variables, such as attendance, learning methods, previous scores, or assignment performance.
- Use a larger dataset to improve model reliability.
- Perform further feature analysis to identify additional factors affecting student performance.

---

## Technologies Used

Programming Language:
- Python

Libraries:
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

Tools:
- Jupyter Notebook
- Google Colab
- GitHub

Methods:
- Data Cleaning
- Exploratory Data Analysis (EDA)
- Regression Modeling
- Model Evaluation

---

## Project Presentation

The project presentation is available here:

`presentation/Student_Performance_Prediction.pdf`

The presentation contains:

- Background and analytical questions
- Dataset understanding
- Data quality checking
- Exploratory data analysis
- Modeling methodology
- Model comparison
- Result interpretation
- Limitations and conclusion
