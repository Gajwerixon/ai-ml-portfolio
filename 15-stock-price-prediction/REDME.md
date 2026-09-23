### Project Summary
In this project, I built a time series model to predict Netflix stock prices using historical market data. This was my first project with time series forecasting and recurrent neural networks, which helped me understand how sequential data can be prepared and used for prediction.

I explored the dataset, analyzed price trends and feature correlations, and then split the data chronologically into training, validation, and test sets. I scaled the features and created 60-day sequences, using the previous 60 trading days to predict the next day's closing price.

I implemented an LSTM model using PyTorch with MSE loss, the Adam optimizer, validation, and early stopping. The model's predictions followed the actual price trend reasonably well, although there is still room for improvement.

Overall, this project gave me a practical understanding of time series preprocessing, sequence creation, LSTM architecture, and model evaluation. In next project I will implement a GRU model and compare its performance with the LSTM.