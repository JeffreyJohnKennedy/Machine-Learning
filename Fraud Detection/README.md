# Fraud Detection in Auto Insurance Claims

## Overview

Fraud detection is a critical challenge in many industries, including auto insurance claims, health insurance claims, credit card transactions, and financial transactions. This project focuses on detecting fraudulent transactions in auto insurance claims using various machine learning techniques. The dataset comes from an actual auto insurance company, with each record representing an insurance claim. The final column indicates whether the claim is fraudulent or not.

## Project Focus

This project demonstrates a step-by-step approach to building, tuning, and evaluating classification models for fraud detection, with the following key components:

### 1. Exploratory Data Analysis (EDA) & Pre-Processing
Initial data exploration and preprocessing steps are performed to clean and transform the dataset for model training.

### 2. Basic Decision Tree Model
A simple decision tree classifier is implemented and evaluated on the dataset as a baseline model for fraud detection.

### 3. Random Search for Decision Tree
Hyperparameter tuning is conducted using **RandomizedSearchCV** to identify the optimal parameters for the decision tree model.

### 4. Grid Search for Decision Tree
An exhaustive search using **GridSearchCV** is carried out to further fine-tune the performance of the decision tree model.
