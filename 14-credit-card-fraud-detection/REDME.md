## Project Summary
This project focused on detecting fraudulent credit card transactions using machine learning techniques. The dataset was highly imbalanced, with fraudulent transactions representing only a very small fraction of all transactions, making fraud detection a challenging classification problem.

Three different approaches were explored:
* **XGBoost** — a supervised learning model trained to distinguish between legitimate and fraudulent transactions.
* **XGBoost + SMOTE** — SMOTE was used to generate synthetic fraudulent transactions and reduce the class imbalance in the training data.
* **Isolation Forest** — an unsupervised anomaly detection algorithm used to identify unusual transactions without using fraud labels during training.

The models were evaluated using **Precision, Recall, F1-score, PR-AUC, and Confusion Matrix**. Accuracy was not treated as the main metric because the strong class imbalance makes it less informative for this problem.

The experiments showed that **XGBoost provided a strong balance between detecting fraudulent transactions and limiting false positives**. SMOTE increased the model's recall, allowing it to detect more fraud cases, but also significantly increased the number of false positives. Isolation Forest was able to detect many fraudulent transactions despite being trained without labels, but it generated a very large number of false positive predictions.

Overall, the project demonstrated the importance of choosing appropriate evaluation metrics and handling class imbalance when working with real-world fraud detection problems. It also showed that improving fraud detection is often a trade-off between **recall and precision**, rather than simply maximizing accuracy.