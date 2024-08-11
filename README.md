# House Prices Prediction - README

## Overview

This project is focused on predicting house prices using advanced regression techniques. We leverage both Linear Regression and Random Forest models to predict house prices based on key features of the properties. The dataset used is from the Kaggle competition ["House Prices: Advanced Regression Techniques"](https://www.kaggle.com/c/house-prices-advanced-regression-techniques).

## Project Structure

The repository is organized as follows:

- `train.csv`: Training dataset containing features and the target variable (`SalePrice`).
- `test.csv`: Test dataset containing features for which predictions are to be made.
- `test_predictions.csv`: Output file containing predictions made by both Linear Regression and Random Forest models on the test data.
- `house_price_prediction.py`: The main script that contains the data processing, model training, evaluation, and visualization.
- `README.md`: This file, which provides an overview of the project.

## Setup and Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/house-prices-prediction.git
   cd house-prices-prediction
   ```

2. **Install the required Python packages**:
   Make sure you have Python installed. You can install the required packages using `pip`:
   ```bash
   pip install pandas matplotlib seaborn scikit-learn
   ```

3. **Download the dataset**:
   You need to download the `train.csv` and `test.csv` files from the [Kaggle competition page](https://www.kaggle.com/c/house-prices-advanced-regression-techniques) and place them in the project directory.

## How to Run the Project

1. **Run the Python script**:
   Execute the script to perform data preprocessing, model training, evaluation, and visualization:
   ```bash
   python house_price_prediction.py
   ```

2. **Output**:
   - The script will generate a CSV file named `test_predictions.csv`, which contains the predictions for the test data.
   - Several visualizations will be displayed, including the distribution of the target variable, correlation matrix, and residuals.

## Models Used

- **Linear Regression**:
  - A simple linear model that assumes a linear relationship between the features and the target variable.
  - Metrics:
    - Mean Squared Error (MSE): A measure of the average of the squares of the errors.
    - R-squared: The proportion of the variance in the dependent variable that is predictable from the independent variables.

- **Random Forest Regressor**:
  - An ensemble learning method that uses multiple decision trees to predict the target variable.
  - Metrics:
    - Mean Squared Error (MSE)
    - R-squared

## Visualizations

1. **Distribution of Sale Price**:
   - Shows the distribution of the target variable `SalePrice` in the training data.
   
2. **Correlation Matrix**:
   - Displays the correlation between `SalePrice` and selected features (`LotArea`, `BedroomAbvGr`, `totalnumbdrm`).

3. **Predicted vs Actual Sale Price**:
   - Scatter plots comparing the predicted sale prices with actual sale prices for both Linear Regression and Random Forest models.

4. **Residuals Distribution**:
   - Histograms showing the distribution of residuals (errors) for both Linear Regression and Random Forest models.

