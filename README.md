# Titanic Survival Prediction

This is a machine learning project to predict the survival of passengers on the Titanic. The dataset used in this project contains information about the passengers such as their age, sex, fare, and whether they survived or not.

## Libraries Used
- pandas
- numpy
- matplotlib.pyplot
- seaborn
- sklearn

## Data Cleaning
Before starting the analysis, the dataset was cleaned to handle missing values and convert categorical variables to numeric values.

### Missing Data
- The `deck` column had a large number of missing values, so it was dropped from the dataset.
- The `age` column had some missing values. The missing values were filled with the mean age of passengers in the same gender and passenger class.
- The `embarked` column had a few missing values. The missing values were filled with the mode value of the column.

### Feature Engineering
- Categorical variables like "sex" and "embarked" were converted to numerical values using one-hot encoding.
- New features like "family_count", "age_bin", and "fare_bin" were created to extract more information from the existing columns.

## Models Used
Three different models were used to predict the survival of passengers:

### 1. Logistic Regression
- The accuracy of the logistic regression model was 81.37%.

### 2. K Nearest Neighbors (KNN)
- The accuracy of the KNN model was 79.33%.

### 3. Decision Tree
- The accuracy of the decision tree model was 78.21%.

## Conclusion
Based on the accuracy scores, it can be concluded that the Logistic Regression model performed slightly better than the other two models in predicting the survival of passengers on the Titanic. 

However, it is worth noting that these models can be further optimized by tuning hyperparameters and trying different approaches for feature engineering.
