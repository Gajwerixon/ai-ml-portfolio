## Project Summary
In this project, I built a weekly sales forecasting model using the Walmart Sales Forecasting dataset and a PyTorch LSTM neural network.

I performed exploratory data analysis, cleaned and merged the datasets, handled missing values, encoded categorical features, and created cyclic time features. The data was split chronologically to prevent data leakage, and 12-week sequences were created for each Store and Department combination.

The final model combined an LSTM with Store and Department embeddings. Early stopping was used to prevent overfitting and save the best-performing model.

On the unseen test data, the model achieved an **MAE of $7,859**, **RMSE of $12,221**, and **R² of 0.692**. The model was able to capture the general sales trend, although individual predictions were often above or below the actual values.

Overall, the model provides a solid baseline, with further improvements possible through longer sequences, additional LSTM layers, dropout, and better feature engineering.