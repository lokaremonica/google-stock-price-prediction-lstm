# 📈 Google Stock Price Prediction using LSTM

## 📌 Overview

This project implements a **Long Short-Term Memory (LSTM)** model to predict Google’s stock prices based on historical "Open" price data. The model processes time-series data, trains over 2000 epochs, and evaluates performance on training and test datasets.

The implementation covers **data preprocessing, sequence creation, model training, evaluation, and visualization**.

---

## 🚀 Features

* **Data Preprocessing**:

  * Min-Max normalization
  * Sequence creation with 60-day lookback window
  * Train-test split (80-20 ratio)

* **Model Architecture**:

  * LSTM with 2 layers, 50 hidden units
  * Linear output layer
  * Trained with Adam optimizer and MSE loss

* **Training & Evaluation**:

  * 2000 training epochs
  * RMSE metrics for training & testing
  * Visualization of predictions vs. actual prices

* **Performance**:

  * Final Training RMSE: **\$4.30**
  * Final Testing RMSE: **\$28.76**
  * Captures overall trends well but shows overfitting after \~700 epochs

---

## 📊 Results & Insights

* **Best Epoch Range**: 100–200
* **Overfitting** observed after epoch 700
* Model predicts general price movements well but struggles with exact price values
* Suitable for **trend forecasting** rather than exact predictions

---

## 🛠️ Technologies Used

* Python
* PyTorch
* Pandas, NumPy, Matplotlib
* scikit-learn
