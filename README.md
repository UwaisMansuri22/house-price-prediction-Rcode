# Housing Price Prediction using XGBoost

This repository contains the implementation of a machine learning project aimed at predicting housing prices based on key features from the dataset. The project uses the **XGBoost** algorithm for regression and includes various steps such as data preprocessing, feature selection, model training, hyperparameter tuning, and evaluation.

## Table of Contents
1. [Overview](#overview)
2. [Features](#features)
3. [Setup and Usage](#setup-and-usage)
4. [Model Details](#model-details)
5. [Results](#results)
6. [File Structure](#file-structure)
7. [Contributing](#contributing)
8. [License](#license)

## Overview
Housing price prediction is a regression task where the goal is to estimate the price of a house based on its characteristics. This project leverages the **XGBoost** algorithm due to its performance and flexibility in handling structured data.

### Key Steps
- Data preprocessing and cleaning
- Exploratory Data Analysis (EDA)
- Feature engineering and selection
- Model training and hyperparameter optimization
- Cross-validation for robustness
- Final predictions and evaluation

## Features
The project includes the following:
- Feature selection based on correlation analysis
- Training and validation dataset split
- Implementation of XGBoost with tuned hyperparameters
- Cross-validation for better generalization
- Saving predictions to a CSV file

## Setup and Usage
1. Clone the repository:
```bash
git clone https://github.com/UwaisMansuri22/house-price-prediction-Rcode.git
cd house-price-prediction-Rcode

2.	Install required libraries:
	•	R
	•	R packages: xgboost, dplyr, ggplot2, corrplot
To install the packages, run the following command in your R console:

install.packages(c("xgboost", "dplyr", "ggplot2", "corrplot"))

3.	Run the notebook:
Open the .ipynb file in Jupyter Notebook or RStudio and execute the cells sequentially to replicate the workflow.
	4.	Generate predictions:
	•	Ensure the test data file is correctly formatted and placed in the data/ directory.
	•	Run the notebook to save predictions in a CSV file named house_regression_result.csv.

Model Details
	•	Algorithm: XGBoost (Extreme Gradient Boosting)
	•	Parameters:
	•	booster: gbtree
	•	objective: reg:squarederror
	•	max_depth: Tuned for optimal performance
	•	eta: Learning rate tuned for better convergence
	•	subsample and colsample_bytree: Regularization techniques to prevent overfitting
	•	Early stopping based on validation performance

Results
	•	Validation Root Mean Squared Error (RMSE): ~28,649
	•	The model predictions for the test dataset are saved in house_regression_result.csv.

File Structure
housing-price-prediction/
│
├── Final_Project_DS636.ipynb   # Main notebook
├── data/                       # Dataset folder
│   ├── train.csv               # Training data
│   ├── test.csv                # Test data
│
├── house_regression_result.csv # Final predictions
└── README.md                   # Project documentation

Contributing

Feel free to submit issues or pull requests. Contributions are welcome!

License

This project is licensed under the MIT License. See the LICENSE file for details.