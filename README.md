# Recipe Rating Prediction

This project aims to predict the ratings of recipes based on various features such as user engagement metrics and text reviews. The dataset used for this project contains information about recipes along with user ratings and comments.

## Dataset Description

The dataset consists of two main files:

- `train.csv`: Contains training data with features and corresponding ratings.
- `test.csv`: Contains testing data with features to be used for prediction.

## Features

The features used for prediction include:

- User engagement metrics: such as Reply Count, Thumbs Up Count, Thumbs Down Count, and User Comment Count.
- Text reviews: Reviews provided by users for each recipe.

## Data Preprocessing

- Feature engineering: Date features were extracted from timestamps, and categorical variables were encoded.
- Data preprocessing pipeline: A pipeline was used to preprocess numerical and text features separately.
- Feature selection: SelectKBest method was used to select the top features.

## Exploratory Data Analysis (EDA)

EDA was performed to gain insights into the dataset, including:

- Frequency of ratings
- Distribution of user reputation by ratings
- Correlation matrix of engagement metrics with ratings
- Outlier detection in engagement metrics

## Machine Learning Models

Three machine learning models were evaluated for predicting recipe ratings:

1. Logistic Regression
2. Random Forest Classifier
3. K-Nearest Neighbors (KNN)

Hyperparameter tuning was performed using grid search, and the models were evaluated using cross-validation.

## Results and Conclusion

Random Forest Classifier yielded the highest cross-validation score, indicating its suitability for predicting recipe ratings. Logistic Regression served as a baseline model, while KNN also showed competitive performance.

In conclusion, Random Forest Classifier is recommended as the final model for predicting recipe ratings due to its balance between performance and model complexity.

## File Description

- `submission.csv`: Contains the predicted ratings for the test dataset.

## Instructions for Running the Code

1. Install the required libraries mentioned in `requirements.txt`.
2. Run the Jupyter notebook or Python script provided.
3. Ensure the dataset files `train.csv` and `test.csv` are placed in the appropriate directory.

## Acknowledgements

The dataset used in this project is sourced from [Kaggle](https://www.kaggle.com/).
