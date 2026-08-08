# Titanic Survival Prediction

## Project Overview

This project predicts whether a passenger survived the Titanic disaster using Machine Learning.

## Dataset

The dataset contains information about Titanic passengers.

The main features used in the project are:
- Pclass: Passenger class
- Sex: Passenger gender
- Age: Passenger age
- SibSp: Number of siblings or spouses aboard
- Parch: Number of parents or children aboard
- Fare: Passenger ticket fare
- Embarked: Port of embarkation

The target variable is `Survived`:
- 0 = Did not survive
- 1 = Survived

## Machine Learning Models

Two classification models were trained and compared:

1. Logistic Regression
2. Decision Tree (max_depth=4)

## Model Evaluation

Cross-validation was used to compare the models.

| Model | Validation Accuracy | Cross-Validation Accuracy |
|---|---:|---:|
| Logistic Regression | ~0.80 | 0.8193 |
| Decision Tree | 0.8324 | 0.8249 |

The Decision Tree was selected as the final model because it achieved better performance than Logistic Regression.

## Kaggle Result

The final Decision Tree submission achieved a Kaggle score of approximately **0.76555**.

## Conclusion

The results showed that passenger gender and passenger class were among the most influential factors in survival prediction.

Feature engineering, including extracting passenger titles, also helped improve the model.

## Future Improvements

Possible future improvements include:
- Trying Random Forest or XGBoost
- Hyperparameter tuning
- Further feature engineering
- Developing an interactive web application
