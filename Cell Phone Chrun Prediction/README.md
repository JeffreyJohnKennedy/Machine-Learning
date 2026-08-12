# Cell Phone Churn Prediction Problem

## Project Summary

This project addresses a binary classification problem, aiming to predict whether a customer will churn (0 or 1) using various machine learning models. The dataset includes 1695 training instances and 375 testing instances, with 24 features each. Key preprocessing steps involved encoding categorical variables and analyzing class distributions.

## Key Components

### 1. Exploratory Data Analysis (EDA) & Preprocessing
- No missing values in the dataset.
- Categorical variables (`CONVB`, `SEX`, `SPORTS`, `ARTS`, `TRAVEL`, `EDUC`) were encoded.
- Class distribution revealed more non-churners (0: 1052) compared to churners (1: 643).

### 2. Base Models
- Initial models included Decision Tree (DT), K-Nearest Neighbors (KNN), Linear SVC, and MLP.
- **Decision Tree (DT)** and **KNN** performed best for predicting the majority class (non-churners).
- **Linear SVC** had the highest recall for the minority class (churners).
- **MLP classifier** did not perform well in this scenario.

### 3. Hyperparameter Tuning
- Hyperparameter tuning was performed on the Decision Tree using a random search.
- **Best parameters** identified: `{'min_samples_split': 10, 'max_leaf_nodes': 19, 'max_features': 22, 'max_depth': 9, 'criterion': 'gini'}`.
- Top 5 features were extracted, though hyperparameter tuning did not significantly improve minority class prediction.

### 4. Stacking
- Combined the predictions of the four base models using majority voting.
- Used **Random Forest** as a meta-model for stacking.
- Stacking results were similar to the individual base models and did not improve minority class prediction significantly.

## Conclusion
- The models (DT, KNN, tuned DT, stacked model) were generally good at predicting the majority class, with high accuracy.
- However, none of the models achieved perfect recall for the minority class (churners), with two misclassifications.
- Overall, the Decision Tree
