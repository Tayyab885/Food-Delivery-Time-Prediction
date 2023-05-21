# Food Delivery Time Analysis and Prediction

This repository contains a Jupyter Notebook that analyzes the factors affecting food delivery time and builds a prediction model based on those factors. The notebook uses Python and various libraries for data analysis, visualization, and machine learning.

## Dataset

The dataset used in this analysis is stored in the file "deliverytime.txt". It contains information about food delivery, including delivery person details, ratings, location coordinates, order type, vehicle type, and the time taken for delivery.

## Notebook Contents

The notebook includes the following sections:

### 1. Importing Basic Libraries

In this section, the necessary libraries for data analysis and visualization are imported, including pandas, numpy, matplotlib.pyplot, seaborn, and the inline magic command for inline plotting.

### 2. Importing the Dataset

The dataset is imported using the pandas library and stored in a DataFrame called "df". The first few rows of the dataset are displayed using the `head()` function.

### 3. Dataset Information

This section provides information about the dataset, including the number of rows and columns, the data types of each column, and memory usage.

### 4. Checking Null Values

This section checks for any missing values in the dataset by using the `isnull().sum()` function. It shows the number of null values in each column.

### 5. Calculating Distance Between Two Latitudes and Longitudes

The haversine formula is used in this section to calculate the distance between two locations based on their latitude and longitude coordinates. The formula is implemented as a function called `haversine()`, which takes latitude and longitude values as input and returns the distance in kilometers.

### 6. Data Exploration

In this section, various visualizations are created to explore the relationships between different variables and the delivery time. Two scatter plots are generated to analyze the relationship between distance and delivery time, delivery person age and delivery time, and delivery person ratings and delivery time. Additionally, a box plot is created to compare the delivery time based on the type of vehicle and type of order.

### 7. Food Delivery Time Prediction Model

This section builds a prediction model using the Long Short-Term Memory (LSTM) algorithm from the Keras library. The model takes the delivery person's age, ratings, and distance as input features and predicts the delivery time. The model architecture is defined using the Sequential API from Keras and is trained on the dataset.

### 8. Food Delivery Time Prediction

The trained model is used in this section to predict the delivery time based on user input for the delivery person's age, ratings, and distance. The predicted delivery time is displayed as output.

## Usage

To use this notebook, follow these steps:

1. Ensure that you have Python installed along with the required libraries mentioned in the notebook.
2. Download the dataset file "deliverytime.txt" and place it in the same directory as the notebook.
3. Open the notebook using Jupyter Notebook or any compatible environment.
4. Run each cell sequentially to execute the code and see the results.
5. Modify the code or add additional analysis as per your requirements.
