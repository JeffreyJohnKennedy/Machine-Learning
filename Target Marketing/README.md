# Targeted Marketing

## Overview

There are two main approaches to enterprise marketing:
1. **Mass campaigns**, targeting a broad range of general customers.
2. **Directed marketing**, focusing on a specific set of customers.

In today's competitive environment, mass campaigns are not as productive. However, directed marketing poses its own challenges, especially when it comes to identifying potential customers. Fortunately, data mining (DM) techniques can assist in overcoming these challenges.

## Dataset

The dataset is from a Portuguese banking institution's direct marketing campaign, aimed at selling term deposits to their customers. This can be viewed as a form of cross-selling. The campaign primarily used phone calls to contact customers, and the dataset includes general customer information, details of the contacts, and the output variable `y`, indicating whether a customer subscribed to a term deposit.

## Steps

### 1. Exploratory Data Analysis (EDA) & Pre-Processing
Initial data exploration and preprocessing steps are carried out to clean and transform the dataset for model training.

### 2. Basic Decision Tree Model
A simple decision tree classifier is implemented and evaluated on the dataset as a baseline model.

### 3. Random Search for Decision Tree
Hyperparameter tuning is performed using **RandomizedSearchCV** to find the optimal parameters for the decision tree model.

### 4. Grid Search for Decision Tree
An exhaustive hyperparameter search is conducted using **GridSearchCV** to further fine-tune the decision tree's performance.
