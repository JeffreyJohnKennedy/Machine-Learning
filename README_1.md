# Machine Learning Coursework

A collection of machine learning projects completed as part of my ML coursework. Each project tackles a real-world classification or regression problem, walking through exploratory data analysis, preprocessing, model building, hyperparameter tuning, and (in most cases) ensemble learning via stacking.

## Projects

| Project | Type | Problem | Key Techniques |
|---|---|---|---|
| [Cell Phone Churn Prediction](./Cell%20Phone%20Chrun%20Prediction) | Classification | Predict whether a customer will churn | Decision Tree, KNN, Linear SVC, MLP, hyperparameter tuning, stacking |
| [Fraud Detection](./Fraud%20Detection) | Classification | Detect fraudulent auto insurance claims | Decision Tree, SMOTE, RandomizedSearchCV, GridSearchCV |
| [Homesite Quote Conversion](./Homesite%20Quote%20Conversion) | Classification | Predict quote-to-policy conversion (Kaggle) | SMOTE for imbalanced data, ensemble stacking (5+ models) |
| [House Price Prediction](./House%20Price%20Prediction) | Regression | Predict residential home prices in Ames, Iowa (Kaggle) | Feature engineering, Random Forest, Gradient Boosting, stacking |
| [Santander Customer Satisfaction](./Santander-Customer-Satisfaction) | Classification | Predict customer satisfaction on a highly imbalanced dataset | SMOTE, F1/ROC-AUC evaluation, high-dimensional feature handling |
| [Target Marketing](./Target%20Marketing) | Classification | Predict term deposit subscription for a bank's directed marketing campaign | Decision Tree, RandomizedSearchCV, GridSearchCV |

Each project folder contains its own `README.md` with a detailed write-up and a `notebook.ipynb` with the full implementation.

## Tech Stack

- **Language:** Python
- **Core libraries:** `pandas`, `numpy`, `scikit-learn`, `imbalanced-learn` (SMOTE), `matplotlib`, `seaborn`, `vecstack`
- **Environment:** Jupyter / Google Colab notebooks

## Common Themes Across Projects

- **Imbalanced data handling** — several projects deal with skewed class distributions and use SMOTE to oversample the minority class.
- **Model comparison** — baseline models (Decision Tree, KNN, SVM, MLP, Random Forest, Gradient Boosting) are compared on standard metrics (accuracy, precision, recall, F1, ROC-AUC).
- **Hyperparameter tuning** — `RandomizedSearchCV` and `GridSearchCV` are used to optimize model performance.
- **Ensemble learning** — several projects use one-layer stacking to combine multiple base models into a stronger meta-model.

## Getting Started

Each notebook can be run independently:

```bash
git clone https://github.com/<your-username>/Machine-Learning.git
cd "Machine-Learning/<project-folder>"
pip install pandas numpy scikit-learn imbalanced-learn matplotlib seaborn vecstack
jupyter notebook notebook.ipynb
```

Some notebooks were originally run in Google Colab and mount Google Drive for data access — swap that step out for a local file path if running elsewhere.

## Author

Coursework projects completed as part of a Machine Learning course.
