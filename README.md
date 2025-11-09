# Customer-Churn-Prediction-project
Project Overview

Predict whether a telecom customer will churn using a neural network (ANN).
The model uses customer demographics, account info, and service usage as features.

Dataset

Source: Telco Customer Churn Dataset

Rows / Columns: 7043 × 21

Target: Churn (Yes = 1, No = 0)

Preprocessing

Drop customerID.

Convert Churn to binary (0/1).

One-hot encode categorical features.

Convert TotalCharges to numeric and fill missing values.

Train/test split: 80% / 20%.

Standardize numeric columns (SeniorCitizen, tenure, MonthlyCharges, TotalCharges).

Model

Sequential ANN

Hidden layers:

Dense(3, activation='relu')

Dense(3, activation='relu')

Output layer: Dense(1, activation='sigmoid')

Loss: binary_crossentropy

Optimizer: adam

Metrics: Accuracy

Epochs: 100

Batch size: 32

Training & Evaluation

Model trained on 80% of data, validated on 20%.

Prediction threshold: 0.5

Test accuracy: replace with your result

How to Run

Clone the repo:

git clone <your-repo-url>


Install dependencies:

pip install pandas numpy scikit-learn matplotlib seaborn tensorflow


Run the notebook/script.

Future Improvements

Add dropout to reduce overfitting

Experiment with more neurons/layers

Tune hyperparameters for better performance

Plot training and validation curves

References

Telco Customer Churn Dataset

TensorFlow Keras Documentation
