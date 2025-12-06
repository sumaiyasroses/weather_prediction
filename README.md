# weather_prediction
Seattle Weather Temperature Prediction
          This project uses a neural network regression model to predict the average daily temperature in Seattle based on historical weather data. The model is built using TensorFlow/Keras, with preprocessing and evaluation handled by Pandas and scikit-learn.

Workflow
Load seattle-weather.csv
Create target variable:
         temperature = (temp_max + temp_min) / 2
Preprocess: drop unused columns, scale features (MinMaxScaler)

Split into train/test sets
Train a dense neural network
Evaluate using MAE, MSE, RMSE, R²
Visualize loss curves and predicted vs actual values
Predict temperature for the most recent record

Model Architecture
Dense(64, relu)
Dense(32, relu)
Dense(1)
Loss: MSE
Optimizer: Adam

Outputs
Training & validation loss plot
Final performance metrics
Scatter plot (actual vs predicted)
Single-sample temperature prediction

How to Run:
1.Install dependencies:
pip install numpy pandas matplotlib scikit-learn tensorflow

2.Run the script:
python temperature_prediction.py

