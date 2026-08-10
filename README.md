Delivery Time Prediction
Tech Stack: Python, TensorFlow / Keras, Pandas, Scikit-Learn, NumPy

Environment: Google Colab

About The Project
This project is a machine learning regression model built to estimate food delivery times. Using a 3-Layer Deep Learning Neural Network, the system analyzes various real-world factors to predict the exact number of minutes a delivery will take.

Unlike classification problems, this regression model outputs a continuous numerical value, making it ideal for forecasting and logistics planning.

Features
Synthetic Dataset Generation: Automatically creates a 1,000-record dataset simulating distance, traffic conditions, food preparation time, and courier experience.

Data Normalization: Uses StandardScaler to ensure all features are weighted equally, preventing scale imbalances during neural network training.

Regression Architecture: Implements a neural network with a linear activation function in the output layer and utilizes Mean Squared Error (MSE) and Mean Absolute Error (MAE) for evaluation.

Live Order Estimation: Includes a built-in testing script to predict delivery times for new, incoming orders in real-time.

How to Run (Google Colab)
Generate the Dataset: Run the first data generation script to create and save delivery_data.csv in your environment.

Train the Model: Run the neural network script. The model will split the data, scale the features, and train for 25 epochs.

Test with Live Data: The end of the script simulates a real-time order to demonstrate the model's predictive capabilities.

Model Architecture
Input Layer: 4 Features (distance_km, traffic_index, prep_time_min, courier_exp_yrs)

Hidden Layer: 16 Neurons (Activation: ReLU)

Output Layer: 1 Neuron (Activation: Linear to output continuous numerical values)

Evaluation Metrics: MSE (Loss), MAE (Mean Absolute Error)

Future Enhancements (Integration)
Export the trained model as a .keras file.

Wrap the model in a backend REST API using Python (FastAPI/Flask).

Containerize the backend service using Docker and integrate it into a CI/CD pipeline to serve predictions for a full-stack web application.
