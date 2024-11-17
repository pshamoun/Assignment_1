Tesla Stock Price Prediction using Recurrent Neural Networks (RNN) 

This project implements a Recurrent Neural Network (RNN) using PyTorch to predict Tesla's closing stock price based on historical data and engineered features. The model explores various hyperparameters and evaluates the performance of different configurations.

The assignment required us to:

Build, train, and evaluate an RNN using PyTorch.
Use a minimum of two hidden layers in the RNN architecture.
Experiment with at least three different sets of hyperparameters (e.g., number of layers/neurons, activation functions, epochs, learning rates, etc.).
Include the following steps in the implementation:
Feature Selection
Feature Engineering (if necessary)
Standard ML Preprocessing
#Train-Test Split
#Defining an RNN Architecture
#Creating a Training Loop
#Training the Model
#Experimenting with Hyperparameters
#Evaluating the Model

1. Feature Engineering
Engineered features include:

Lag_1: Previous day's closing price.
MA_14: 14-day moving average of the closing price.
Volatility_14: Standard deviation over the past 14 days.

2. Preprocessing
Data was normalized using Min-Max Scaling to improve training stability.
The dataset was split into training, validation, and test sets with an 80-10-10 ratio.

4. RNN Architecture
The base RNN consisted of:
Input Size: Number of features.
Hidden Size: 42 neurons.
Layers: 2 hidden layers.
Output Size: 1 (closing price prediction).
Three additional configurations of hyperparameters were explored for experimentation.

6. Training
The model was trained for 50 epochs with a batch size of 32.
Training and validation losses were logged during each epoch.

8. Evaluation
The model was evaluated on the test set using:
Mean Squared Error (MSE)
Mean Absolute Error (MAE)
Predictions were visualized against actual prices to assess performance.
