# Presenting the Deep learning for BTC

This repository contains programs leveraging neural networks to predict BitCoin prices. Both models use a sequential LSTM model with three layers (dropout fraction of .2), adam for the optimizer, and mean squared error for the loss factor. 

The lstm_stock_predictor_closing program uses closing prices of BitCoin in the model. This model contains 5 units and a batch size of 1. It is a very accurate model with a loss of only 0.0038. 

The lstm_stock_predictor_fng program uses Fear and Greed (FNG) index values in the model. This model contains 50 units and a batch size of 5. 

Same inputs as the closing price model (5 units and batch size of 1) does not produce better output hence increasing the units and batch size improved the model's accuracy. 
However, this model is overall far less accurate than the other, with a loss of 0.0482.

In conclusion, closing prices are a much better source of data than FNG index values for predicting BitCoin price movements.