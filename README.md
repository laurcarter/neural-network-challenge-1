# Neural Network Challenge 1

## Overview
This project uses a deep learning model to predict student loan repayment success and explores the creation of a recommendation system for student loans. It covers data preparation, model training, evaluation, and future considerations.

---

## Features

### Data Preparation
- **Target Dataset (`y`)**: Extracted from the `credit_ranking` column.
- **Features Dataset (`X`)**: Includes all other columns.
- **Data Splitting**: Training and testing sets created.
- **Feature Scaling**: Applied `StandardScaler` to normalize the data.

### Model Creation and Evaluation
- **Neural Network Design**:
  - Two hidden layers with ReLU activation.
  - One output layer with a sigmoid activation function.
- **Model Training**:
  - Compiled using the `binary_crossentropy` loss function, `adam` optimizer, and accuracy metric.
  - Trained for 50 epochs.
- **Model Evaluation**:
  - Evaluated on test data for accuracy and loss.
  - Saved as `student_loans.keras`.

### Predictions
- **Model Reloading**: Reloaded the saved model.
- **Predictions**:
  - Binary predictions generated for test data.
  - Classification report generated to assess precision, recall, and F1-score.

### Recommendation System Discussion
- **Data Collection**:
  - Demographics, educational details, loan history, credit scores, and location.
- **Filtering Method**:
  - Context-based filtering to personalize recommendations.
- **Challenges**:
  - Addressing privacy concerns and mitigating biases in data.
```
