## Project Summary
In this project, I built a machine learning system to predict customer churn using a bank customer dataset. The goal was to identify customers who are likely to leave the bank based on their demographic information and banking activity. I tested four classification models: **Logistic Regression, Decision Tree, Random Forest, and Gradient Boosting**.

The models were evaluated using **Accuracy, Precision, Recall, F1-score and Confusion Matrix**. The results showed that Accuracy alone was not sufficient because the dataset was imbalanced, making Recall and F1-score especially important for evaluating churn detection.

Among the tested models, **Gradient Boosting achieved the best overall performance**, including an F1-score above 60%. This showed that ensemble-based boosting methods were better at balancing the detection of churned and retained customers than the simpler models.