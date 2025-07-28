California Housing Price Prediction using TensorFlow



This project builds a basic regression model using TensorFlow and the California Housing dataset from Scikit-learn. The model is trained to predict median house values in California districts based on demographic and geographic features.

Dataset
Source: sklearn.datasets.fetch_california_housing

Type: Tabular dataset with 8 numerical input features and 1 target output (median house value)

Features Used
MedInc – Median income in block group

HouseAge – Median house age

AveRooms – Average number of rooms

AveBedrms – Average number of bedrooms

Population – Population per block group

AveOccup – Average household occupancy

Latitude – Latitude

Longitude – Longitude

Model Architecture
Input Layer: 8 input features

Hidden Layer: Dense(64 units, ReLU activation)

Output Layer: Dense(1 unit, no activation) – regression output

Preprocessing
Feature normalization using StandardScaler

Data split into training and testing sets (80% train, 20% test)

Training Details
Loss Function: Mean Squared Error (mse)

Metric: Mean Absolute Error (mae)

Optimizer: Adam

Epochs: 10

Validation: Performed on the test set
