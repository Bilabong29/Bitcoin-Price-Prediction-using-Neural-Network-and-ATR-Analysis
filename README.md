# Bitcoin Price Analysis with Neural Network

This notebook presents a comprehensive analysis of Bitcoin price data (`hasil_atr_btc.csv`) using a neural network model to predict trading actions (Buy, Hold, Sell).

The analysis covers the following steps:

1.  **Data Loading**: The dataset is loaded and inspected.
2.  **Preprocessing**: Data cleaning, handling duplicates, normalization of numerical features, and encoding of categorical variables (`Type`, `Label`) are performed.
3.  **Exploratory Data Analysis (EDA)**: Visualizations including boxplots, pairplots, and a correlation heatmap are generated to understand the data distribution, relationships between features, and identify potential outliers or redundant features.
4.  **Data Splitting**: The dataset is split into training and testing sets for model development and evaluation.
5.  **Neural Network Design**: A Sequential Keras model with dense layers and dropout is designed for multi-class classification.
6.  **Model Training & Evaluation**: The neural network is trained on the prepared data, and its performance is evaluated using metrics like accuracy, precision, recall, and F1-score.
7.  **Prediction**: The trained model is used to make predictions on new data samples.
8.  **Hyperparameter Tuning**: A manual grid search is implemented to find the optimal combination of hyperparameters (neurons, learning rate, batch size) for the neural network to improve model performance.

This project demonstrates a practical application of neural networks for financial time series analysis and trading signal prediction.
