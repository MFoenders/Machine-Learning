# 🏡 HousingPrices: Predict if a House is Expensive or Not
Welcome to the Housing Prices Project! In this exciting project, we use data from 80 different features to figure out if a house is expensive or not. This is what we call a binary classification problem, a simple yes-or-no question. Along the way, you'll see how we prepare the data, pick the right model, and fine-tune it for the best results. Excitingly, this project was a big hit and led me to win the competition in my Data Science Bootcamp!

## Data
- housing classification: This is the main dataset we use to create and train our model.
- test: This is a dataset we haven't used before. We use it to test how well our model works. We uploaded its predictions to the platform for checking.
- data description: This file gives detailed information about each feature in the datasets. It helps understand the data better.

## Notebook
- Model Selection Notebook: Explore and compare various machine learning models to identify the most suitable one for our data.
- Model Application & Tuning Notebook: Experience the process of applying the selected model, adjusting its settings, and improving its effectiveness.
- It was with the Random Forest model that I achieved the best results.

## Model Pipeline
- Processing Numerical Data:
  - SimpleImputer: This tool fills in any missing values in numerical data.
- Processing Categorical Data:
  - SimpleImputer: Similar to numerical data, it fills in missing values in categorical data.
  - OneHotEncoding: This changes categorical data into a format that's ready for machine learning.
  - Scaler: I used the Min-Max Scaler to achieve the best results.

## Hyperparameter Tuning
Maximizing my Model's Potential:
- I started with RandomSearchCV, exploring a wide range of settings quickly and efficiently. The parameters we focused on included:
  - 'randomforestclassifier__n_estimators': [200, 300, 400]
  - 'randomforestclassifier__max_depth': [20, 30, 40]
  - 'randomforestclassifier__min_samples_split': [2, 5, 10]
  - 'randomforestclassifier__min_samples_leaf': [1, 2, 4]
- After identifying promising configurations, I used GridSearchCV with a more specific set of parameters for fine-tuning, ensuring our model was adjusted to its optimum performance.

## Final Result
Predicting Unseen Data: When I tested my model on new data (where we didn't know the actual results), it achieved an amazing accuracy of 97.94%. We're really happy with this result, but we're always looking for ways to do even better in the future.


