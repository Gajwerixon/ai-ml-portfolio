# Titanic Survival Prediction

## Project Summary

The goal of this project is to predict whether a passenger survived the Titanic disaster based on demographic, travel, and family-related features.

During EDA, several important patterns were identified. Survival rates differed significantly by sex and passenger class, with women and first-class passengers having substantially higher survival rates. Age and fare also showed useful relationships with survival, while most passengers travelled alone.

During Feature Engineering, several additional features were created, including `FamilySize`, `IsAlone`, `Title`, and `Deck`. Missing values were handled using median and mode imputation, while categorical features were encoded for machine learning models.

Two classification models were trained and compared: **Decision Tree** and **Random Forest**. Both models achieved relatively similar results, with only a few percentage points difference across the main evaluation metrics. Random Forest performed slightly better overall, achieving higher accuracy, precision, and F1 score, while Decision Tree achieved slightly better recall.