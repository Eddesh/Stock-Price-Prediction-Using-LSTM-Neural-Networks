# Stock-Price-Prediction-Using-LSTM-Neural-Networks

## Project Overview
This project develops and fine-tunes Long Short-Term Memory (LSTM) models to predict the stock prices of Apple (AAPL) and AMD based on historical data from 1980 to 2020. The project focuses on three LSTM model architectures, with the second model – a two-layer LSTM with dropout and learning rate scheduling – demonstrating the best performance, effectively handling both steady and volatile stock price trends.

### Dataset Description
The dataset includes daily historical stock price data for AAPL and AMD, covering key features such as open, high, low, close, adjusted close, and volume. Data preprocessing steps include normalizing the values and splitting the dataset into training, validation, and test sets to enable robust model training and evaluation.

### Step 1: Data Preprocessing and Splitting
The data is preprocessed by normalizing stock prices and splitting the dataset into training, validation, and testing sets, ensuring that the model learns and generalizes well. Additionally, the time series nature of the data is preserved through careful splitting.

### Step 2: Model Training
Three LSTM models were trained:

Model 1: A basic single-layer LSTM with 50 units, followed by a Dense output layer.
Model 2: A fine-tuned two-layer LSTM with 100 and 50 units, including dropout and a learning rate scheduler, which achieved the best results.
Model 3: A more complex, three-layer LSTM model with 150, 100, and 50 units, showing improved results but with slightly higher error rates compared to Model 2.
Each model utilizes early stopping to prevent overfitting and to ensure the best weights are used for evaluation.

### Step 3: Prediction and Evaluation
The models’ performance is evaluated using metrics such as Root Mean Square Error (RMSE), Mean Absolute Error (MAE), and Mean Absolute Percentage Error (MAPE). Model 2 performed best on both AAPL and AMD, achieving lower error rates across all evaluation metrics. Visualization of training and validation losses further confirms Model 2’s superior generalization capabilities.

## Testing
The project includes three LSTM models tested on AAPL and AMD data:

1. Model 1: Basic architecture with higher error rates, indicating room for improvement.
2. Model 2: Shows stable training and validation losses, achieving the lowest errors across all metrics.
3. Model 3: Improved performance over Model 1 but slightly less accurate than Model 2.

## Author
Davin Edbert Santoso Halim
