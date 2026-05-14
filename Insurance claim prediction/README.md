# Insurance Claim Prediction

## Project Overview
This project predicts whether a customer is likely to make an insurance claim using machine learning classification models.

## Problem Statement
Insurance companies need to identify customers who are more likely to make claims. This helps in better risk assessment and decision-making.

## Dataset
The dataset contains customer and policy-related information with a highly imbalanced target variable.

Target distribution:
- No Claim: 96.35%
- Claim: 3.64%

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Imbalanced-learn

## Project Workflow
1. Data loading
2. Data cleaning
3. Exploratory data analysis
4. Missing value handling
5. Feature scaling
6. Train-test split
7. Model building
8. Model evaluation
9. Threshold tuning

## Models Used
- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier
- XGBoost Classifier
- Manually Tuned Random Forest
- Threshold-Tuned Random Forest

## Best Model
The Threshold-Tuned Random Forest model was selected because it improved minority class recall.

## Best Model Performance
- Accuracy: 47%
- Recall for Claim Class: 62%
- Precision for Claim Class: 4%
- F1-score for Claim Class: 0.08

## Why Recall Was Prioritized
Since the dataset is highly imbalanced, accuracy alone is misleading. In insurance claim prediction, identifying possible claim cases is more important than only achieving high accuracy.

## Challenges Faced
- Highly imbalanced target variable
- Low minority class recall
- Misleading accuracy score
- High false positives after threshold tuning
- Need for better imbalance handling

## Conclusion
The project shows that threshold tuning can improve recall for the minority class. However, the model still has low precision and requires further improvement before production use.

## Future Improvements
- Apply SMOTE or advanced imbalance handling
- Use proper preprocessing pipelines
- Perform RandomizedSearchCV or GridSearchCV
- Improve precision-recall balance
- Deploy the model using Streamlit