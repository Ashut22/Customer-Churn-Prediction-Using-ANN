# Customer-Churn-Prediction-Using-ANN
This project predicts customer churn using an Artificial Neural Network (ANN) built with TensorFlow and Keras. The model was trained on the **Churn_Modelling.csv** dataset and achieved an accuracy of **86.25%** on the test set.

## Dataset: Churn_Modelling.csv

The dataset contains customer information for a bank, with the goal of predicting whether a customer will leave the bank (churn). Key features include:

- **Geography**: Customer's location (e.g., France, Germany, Spain).
- **Gender**: Male or Female.
- **CreditScore, Balance, Tenure, Age, etc.**: Various financial and demographic details.
- **Exited**: Target variable indicating whether the customer churned (1 = churned, 0 = retained).

## Project Overview

### Data Preprocessing:
- Irrelevant columns were dropped.
- Categorical variables were encoded using one-hot encoding.
- Numerical features were standardized for consistent scaling.

### Model Architecture:
- Three hidden layers, each with 11 neurons and sigmoid activation.
- The output layer uses sigmoid activation for binary classification.

### Training and Optimization:
- The model was compiled with the Adam optimizer and binary crossentropy loss.
- Early stopping and model checkpointing techniques were used to prevent overfitting and save the best-performing model.

### Performance:
- The model achieved an accuracy of **86.25%** on the test set.

## Visualizations

- **Loss Plot**: Training and validation loss were plotted to monitor model convergence.
- **Accuracy Plot**: Accuracy plots were used to track improvements in classification performance over epochs.

## How to Run

1. Install the required libraries: **NumPy**, **Pandas**, **Scikit-learn**, **TensorFlow**, and **Matplotlib**.
2. Place the `Churn_Modelling.csv` file in the project directory.
3. Run the script to preprocess the data, train the model, and evaluate its performance.
