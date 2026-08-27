## Project Summary

A **Logistic Regression model with TF-IDF features** was used as the baseline for Twitter sentiment classification. The model was trained on cleaned tweet text and evaluated on four sentiment classes: **Positive, Negative, Neutral, and Irrelevant**.

The model correctly classified the majority of tweets and provided a solid baseline for the project. The biggest challenge was the **Irrelevant** class, which had a relatively high number of misclassifications. The model also struggled to distinguish between **Positive and Neutral** as well as **Positive and Negative** tweets, where the language can be semantically similar.

Two preprocessing approaches were compared: **basic text cleaning** and **extended cleaning with stopword removal**. Both approaches produced almost identical TF-IDF representations and model performance. This indicates that removing stopwords had very little impact on this dataset. Therefore, the **basic cleaning approach** was selected for the final baseline model due to its simplicity and preservation of more original text information.