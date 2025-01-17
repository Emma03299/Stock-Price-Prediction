# Google Stock Price Analysis/Prediction
Stock Price Prediction
Data Source
https://www.kaggle.com/datasets/surajjoshi26/google-stock-price2004-2023

Two supervised machine learning approaches to predict future stock prices using historical data from Google. 
The dataset contains over 4,000 data points, focusing exclusively on Google's stock. 
For this, we utilized Long Short-Term Memory (LSTM) neural networks and Random Forest models. 
Our approach includes robust handling of outliers and anomalies to ensure the reliability of the predictions. Through comprehensive training and evaluation, we demonstrate the potential of these models to provide valuable insights into stock price trends.

Steps:
Re-coded the Date column using the datetime method. 
Created a remove_outliters method so that any missing values in the dataset were addressed through removal, depending on the extent of missingness and the importance of the feature.
Scaled features to a similar range using techniques like Min-Max scaling to prevent certain features from dominating the learning process
Included additional features for the Random Forest Classifier, which were derived from the original dataset, such as Open-Close price differentials, High-Low price differentials, and rolling statistics of returns, to provide more information for the models to learn from.
Split the dataset into training and testing sets, using a 75-25 ratio and 80-20 ratio, to evaluate model performance and prevent overfitting.

Libraries Used:
Pandas: For data manipulation and analysis, including reading the CSV file, handling missing values, and performing statistical operations.
NumPy: For numerical operations and handling of arrays, especially for feature scaling and transformation.
Seaborn and Matplotlib: For data visualization to create plots and charts for data analysis.
Scikit-learn: For implementing machine learning algorithms, including Random Forest, and preprocessing techniques like Min-Max scaling
Keras: For building and training the LSTM neural network model.
