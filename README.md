# California Housing Price Prediction using TensorFlow

This project demonstrates how to build a basic regression model using TensorFlow and the California Housing dataset. The model predicts median house prices in different districts based on a variety of features such as income, population, and location.

## Overview

* **Goal**: Predict the median house value in California districts.
* **Type**: Supervised Regression Problem.
* **Tool**: TensorFlow (Keras API).

## Dataset

* **Source**: Scikit-learn's California Housing dataset (`fetch_california_housing`)
* **Features**:

  * Median Income
  * House Age
  * Average Rooms
  * Average Bedrooms
  * Population
  * Average Occupancy
  * Latitude
  * Longitude
* **Target**: Median house value (in \$100,000s)

## Data Preprocessing

* Data is split into training and testing sets (80/20 ratio).
* Features are scaled using `StandardScaler` for improved model convergence.

## Model Architecture

* Input Layer with 8 features
* One Hidden Layer with 64 neurons and ReLU activation
* Output Layer with a single neuron (for price prediction)

## Training Configuration

* **Loss Function**: Mean Squared Error (MSE)
* **Optimizer**: Adam
* **Metric**: Mean Absolute Error (MAE)
* **Epochs**: 10
* **Validation**: Uses the test set for validation during training

## Performance

After training for 10 epochs, the model achieves reasonable performance in predicting housing prices. Accuracy metrics may vary depending on initialization and split.

## How to Run

1. Clone the repository.
2. Install required packages: TensorFlow and Scikit-learn.
3. Run the Python script to train and evaluate the model.
