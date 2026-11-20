# SWYNEX – Model Improvement

## Project Overview
This project focuses on improving and validating the Random Forest machine learning model developed in Task 2 using the Titanic dataset.

## Objectives
- Apply feature engineering.
- Perform hyperparameter tuning.
- Validate the model using 5-fold cross-validation.
- Compare the improved model with the previous Random Forest model.

## Dataset
The cleaned Titanic dataset was used for model improvement.

## Feature Engineering
Two new features were created:

- **FamilySize:** Total number of family members travelling with a passenger.
- **IsAlone:** Indicates whether a passenger was travelling alone (1 = Yes, 0 = No).

## Model Improvement Techniques
- Algorithm: Random Forest Classifier
- Hyperparameter tuning: GridSearchCV
- Cross-validation: 5-fold
- Train-test split: 80:20

### Best Hyperparameters
- n_estimators: 100
- max_depth: 10
- min_samples_split: 5
- min_samples_leaf: 2

**Best Cross-Validation F1 Score: 75.51%**

## Model Performance Comparison

| Metric | Task 2 Random Forest | Task 3 Improved Random Forest |
|---|---:|---:|
| Accuracy | 82.12% | 81.01% |
| Precision | 81.36% | 80.70% |
| Recall | 69.57% | 66.67% |
| F1 Score | 75.00% | 73.02% |

## Findings
The improved model achieved an F1 score of 73.02% on the test dataset, compared with 75.00% in Task 2.

Although feature engineering and hyperparameter tuning were applied, the test performance decreased slightly across all four metrics.

This experiment demonstrates that feature engineering and hyperparameter tuning do not always guarantee better test performance. The results were documented to provide an honest comparison.

## Conclusion
The model was successfully improved through feature engineering and GridSearchCV tuning and validated using 5-fold cross-validation. The original Random Forest model from Task 2 performed slightly better on the held-out test dataset.

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
