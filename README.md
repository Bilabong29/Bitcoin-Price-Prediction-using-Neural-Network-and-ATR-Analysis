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

**Result**
![heatmap](https://github.com/user-attachments/assets/999499a0-1c2a-4995-b875-98cbe667347b)
![accuracy_boxplot](https://github.com/user-attachments/assets/416c10ee-dc08-4d50-a0f9-c856ac59a32d)
![training_history](https://github.com/user-attachments/assets/7d9e0c43-fd90-4797-8fbd-cc513063c2b1)
![gridsearch_barplot](https://github.com/user-attachments/assets/0108c3df-f62f-4b30-8f7c-6df5430df509)
![boxplot](https://github.com/user-attachments/assets/98e6f167-09ea-4fd6-a302-903a9a0c3c3a)
![gridsearch_heatmap](https://github.com/user-attachments/assets/66e70e54-2748-49c9-a26b-d36609443a4c)
![accuracy_trend_neurons](https://github.com/user-attachments/assets/74b0817b-6d8c-48f8-92a3-33b1561efb19)
