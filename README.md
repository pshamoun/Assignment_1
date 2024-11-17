Tesla Stock Price Prediction using Recurrent Neural Networks (RNN) 

This project implements a Recurrent Neural Network (RNN) using PyTorch to predict Tesla's closing stock price based on historical data and engineered features. The model explores various hyperparameters and evaluates the performance of different configurations.

The assignment required us to build, train, and evaluate an RNN using PyTorch.
Use a minimum of two hidden layers in the RNN architecture.
Experiment with at least three different sets of hyperparameters (e.g., number of layers/neurons, activation functions, epochs, learning rates, etc.).

Methodology
1. Feature Engineering: engineered features include: Lag_1: Previous day's closing price. MA_14: 14-day moving average of the closing price. Volatility_14: Standard deviation over the past 14 days.
   
2. Preprocessing: data was normalized using Min-Max Scaling to improve training stability. The dataset was split into training, validation, and test sets with an 80-10-10 ratio.
3. RNN Architecture: the base RNN consisted of: Input Size: Number of features. Hidden Size: 42 neurons. Layers: 2 hidden layers. Output Size: 1 (closing price prediction).
Three additional configurations of hyperparameters were explored for experimentation.
5. Training: the model was trained for 50 epochs with a batch size of 32. Training and validation losses were logged during each epoch.
7. Evaluation: the model was evaluated on the test set using: Mean Squared Error (MSE) Mean Absolute Error (MAE)
   Predictions were visualized against actual prices to assess performance.

![image](https://github.com/user-attachments/assets/1fe79964-6bd4-446d-a235-ea00f5b33d8c)

Requirements:
PyTorch
NumPy
Matplotlib
Scikit-learn

