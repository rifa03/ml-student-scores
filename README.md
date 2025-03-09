# Student Scores Prediction using Machine Learning

## Project Description
This project applies machine learning regression techniques to predict student scores based on study hours. It uses three models: Linear Regression, Decision Tree, and Random Forest, comparing their performance using R-squared, Mean Absolute Error (MAE), and Root Mean Squared Error (RMSE).

## Goals
- Understand the relationship between study hours and exam scores.
- Train and compare multiple regression models.
- Evaluate model performance using statistical metrics.
- Gain experience in data preprocessing, visualization, and machine learning.

## Insights
- **Linear Regression** performed well but struggled with non-linearity in the data.
- **Decision Tree Regressor** captured patterns better but had some overfitting tendencies.
- **Random Forest Regressor** provided the best balance between accuracy and generalization.
- **R-squared scores**:
  - Linear Regression: 0.8981
  - Decision Tree: 0.9087
  - Random Forest: 0.9023

## Dependencies
This project requires the following Python libraries:
- `pandas` (Data handling)
- `numpy` (Numerical computations)
- `matplotlib` & `seaborn` (Data visualization)
- `scikit-learn` (Machine learning models)

To install dependencies, run:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

## Advice for Beginners
- Start by exploring the dataset and visualizing relationships.
- Split data properly into training and testing sets to avoid overfitting.
- Try multiple models and compare their performance.
- Use evaluation metrics beyond accuracy, such as RMSE and MAE, to get a complete picture.
- Experiment with hyperparameters in Decision Tree and Random Forest to improve results.
