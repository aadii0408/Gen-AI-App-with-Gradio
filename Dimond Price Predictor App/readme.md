# Diamond Price Predictor
> This application predicts the price of a diamond based on various attributes like carat, cut, color, clarity, and dimensions (length, width, depth). The app is built using Gradio for the interface, scikit-learn for machine learning, and seaborn for loading the dataset.

## Features
- Input Sliders: Allows users to adjust diamond features such as carat, cut, color, clarity, and dimensions.
- Machine Learning Model: A Random Forest Regressor is used to predict the price of diamonds.
- Data Preprocessing: Numeric data is scaled, and categorical data is encoded using OneHotEncoder.
- Real-time Predictions: Users can interactively change values and see price predictions in real-time.
- Visualization: Utilizes Seaborn to load the diamonds dataset, which is built into the app for easy testing and deployment.

## Tech Stack
- Python: Core language used for building the application.
- Pandas: For data manipulation and handling.
- Seaborn: Used to load the diamonds dataset.
- scikit-learn: For machine learning tasks such as data preprocessing and the random forest regression model.
- Gradio: For building an interactive web interface to display inputs and outputs.

## Code Structure
1. Data Preparation:

The diamonds dataset is loaded using Seaborn.
The dataset is split into features (X) and target (y).
Train-test split is performed using train_test_split.

2. Data Preprocessing:

Numerical features such as carat, depth, table, x, y, z are scaled using StandardScaler.
Categorical features such as cut, color, clarity are encoded using OneHotEncoder.

3, Model Building:

A RandomForestRegressor model is used for prediction.
The pipeline includes preprocessing and modeling in one go, ensuring that raw data can be input and processed effectively.

4. Gradio Interface:

Users can input diamond features using sliders and dropdowns.
The interface displays a real-time prediction of the diamond's price.
