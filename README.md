# Haas-Capstone
Customer Churn Prediction Project
# Customer Churn Prediction Project

## Overview

This project focuses on predicting customer churn for a media company. Churn prediction is critical for businesses as it can significantly impact revenue. By accurately predicting churn, companies can take proactive measures to retain customers and improve their services.

## Data

The dataset consists of 8 CSV files containing information about customers, media consumption events, subscription events, and marketing campaigns.

## Methodology

The project uses RandomForestClassifier to model and predict churn. The process includes data cleaning, exploratory analysis, feature engineering, and model evaluation.

## Key Findings

Based on the classification report, we can summarize the key findings for each class (0 and 1), as well as the overall model performance:

Class 0 (Negative Class)
Precision: 76% of the instances predicted as class 0 were actually class 0.
Recall: 90% of the actual class 0 instances were correctly predicted by the model.
F1-Score: The balance between precision and recall for class 0 is 83%, which is relatively high.
Class 1 (Positive Class)
Precision: 67% of the instances predicted as class 1 were actually class 1.
Recall: 41% of the actual class 1 instances were correctly predicted by the model.
F1-Score: The balance between precision and recall for class 1 is 51%, which indicates that the model is less effective at correctly identifying positive cases compared to negative ones.
Overall Model Performance
Accuracy: The model correctly predicted 74% of all cases, which is a decent overall performance but not exceptional.
Macro Average:
Precision: The average precision across both classes is 72%, without taking class imbalance into account.
Recall: The average recall across both classes is 66%, also not considering class imbalance.
F1-Score: The macro-average F1-score is 67%, which gives an equally weighted average for both classes.
Weighted Average:
Precision: The precision is slightly higher at 73% when weighted by the number of instances in each class.
Recall: This matches the overall accuracy of 74%, as it's a weighted measure.
F1-Score: The weighted average F1-score is 72%, which is higher than the macro average, indicating that the model performs better on the more prevalent class.


# Key Observations and Recommendations
The model performs better on class 0 than on class 1, with higher precision, recall, and F1-score.
The recall for class 1 is particularly low, meaning that many positive instances are being missed (false negatives).
Since the weighted average is higher than the macro average for precision and F1-score, we can infer that class 0, which has more instances, is driving the performance of the model, causing potential issues with class imbalance.
The model may benefit from techniques to address class imbalance, such as oversampling the minority class, undersampling the majority class, or using class weights.
The model might be improved with more features, feature engineering, or hyperparameter tuning that could help to better capture the characteristics of class 1.
Depending on the specific application and the costs associated with false positives and false negatives, further model adjustment might be needed to balance recall and precision in a way that aligns with business or application objectives.

## Repository Structure

- `README.md`: This overview and summary of the project.
- `Capstone Project -aa.ipynb`: The Jupyter Notebook containing all the code, analysis, and technical details.
- `data/`: Folder containing the dataset CSV files.

