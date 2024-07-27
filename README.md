# Sentiment Analysis on Social Media Posts

This project implements a sentiment analysis model to classify social media posts as positive or negative. The model uses an LSTM-based neural network to perform this classification.

## Overview

The script reads training and test data, preprocesses the text, builds and trains an LSTM model, and evaluates its performance.

## Requirements

Make sure you have the following Python packages installed:

```bash
pip install pandas numpy scikit-learn tensorflow matplotlib seaborn
```

## Usage

1. **Prepare Data**: Place `train.csv` and `test.csv` in the same directory as the script.

2. **Output**:
   - **`predicted.csv`**: Contains the test data with predicted sentiment labels.
   - Model metrics including accuracy, precision, recall, and F1-score will be printed.
   - A confusion matrix will be displayed to visualize model performance.

## Script Details

- **Data Preprocessing**:
  - Load and preprocess data using pandas and scikit-learn.
  - Encode sentiment labels and prepare text data for the model using tokenization and padding.

- **Model Building**:
  - Create an LSTM model with embedding, LSTM, and dense layers.
  - Compile the model with categorical cross-entropy loss and the Adam optimizer.

- **Training and Evaluation**:
  - Train the model with early stopping to prevent overfitting.
  - Plot training and validation metrics.
  - Predict sentiments on test data and evaluate using accuracy, precision, recall, F1-score, and confusion matrix.

- **Visualization**:
  - Display the confusion matrix using seaborn to illustrate classification results.

## Results

- **Accuracy**: 0.8619
- **Precision**: 0.8632
- **Recall**: 0.8619
- **F1-score**: 0.8618

- **Confusion Matrix**:
  ```
  [[10396  2104]
   [ 1349 11151]]
  ```

