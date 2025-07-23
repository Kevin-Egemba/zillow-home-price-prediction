# Zillow Home Price Prediction

This repository contains an end-to-end data science project that explores, models, and evaluates real estate data to predict home prices using Zillow’s public dataset. This project is a deliverable for coursework in the Boston University M.S. in Data Science program and showcases best practices in exploratory data analysis, regression modeling, and reproducible research.

## Project Overview

Home price prediction is a crucial task in the real estate industry, helping buyers, sellers, and investors make informed decisions. This project leverages the `zillow_dataset.csv` dataset to develop machine learning models that estimate house prices based on property features such as square footage, number of bedrooms/bathrooms, and zip code.

### Main Goals:
- Clean and explore real estate data from Zillow.
- Engineer features for improved predictive performance.
- Train and evaluate regression models (Linear, Ridge, Lasso, Decision Tree).
- Visualize model performance and interpret feature importance.

## Technologies Used

- Python 3.9+
- pandas
- matplotlib & seaborn
- scikit-learn
- statsmodels
- requests (for data download automation)
- JupyterLab (for exploratory and iterative analysis)

## Repository Structure
├── Milestone_01.ipynb # Initial EDA, feature engineering, baseline models
├── Milestone_02.ipynb # Regularized regression, tree models, diagnostics
│── zillow cleaned.csv # Cleaned Zillow dataset used in modeling
├── README.md # Project documentation
├── requirements.txt # Environment dependencies
└── download_zillow.py # Script to download data from BU-hosted URL



## Dataset
The dataset `zillow cleaned.csv` was sourced from BU’s CS505 course materials. It contains housing data including:
- Living area (square feet)
- Number of bedrooms and bathrooms
- Zip code
- Lot size, number of floors, and waterfront/condition indicators
- Price (target variable)

## Modeling Techniques

### Baseline:
- Multiple Linear Regression (OLS)

### Regularized Models:
- Ridge Regression (L2)
- Lasso Regression (L1)

### Tree-Based:
- Decision Tree Regressor (with max depth tuning)

### Evaluation Metrics:
- R² (Coefficient of Determination)
- RMSE (Root Mean Squared Error)
- Residual Plots and Distribution Checks

## Key Insights

- Multicollinearity was addressed using VIF analysis.
- Regularization (Ridge/Lasso) helped control overfitting and improve generalization.
- Decision Trees provided interpretability and localized prediction behavior.
- Price prediction variance was lowest when zip code and square footage were included.

## How to Run
2. Install dependencies
   
1. **Clone this repository**  
   git clone https://github.com/your-username/zillow-home-price-prediction.git
   cd zillow-home-price-prediction

pip install -r requirements.txt



Download the dataset (if not already present)
Run:
python download_zillow.py


Launch JupyterLab and run notebooks

jupyter lab

Kevin Egemba
M.S. in Data Science, Boston University
Email: kegemba@bu.edu
GitHub: github.com/kevinegemba



