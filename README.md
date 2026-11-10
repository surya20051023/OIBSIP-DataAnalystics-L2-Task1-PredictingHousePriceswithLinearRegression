# OIBSIP-DataAnalystics-L2-Task1-Predicting-House-Prices-with-Linear-Regression-
# Task 1: Predicting House Prices with Linear Regression

## Project Overview

This project uses machine learning to predict house sale prices based on features such as living area, overall quality, basement area, garage capacity, construction year, number of bathrooms, neighbourhood, and kitchen quality.

A Linear Regression model is developed using Python and Scikit-learn. The project covers the complete machine learning workflow, including exploratory data analysis, data preprocessing, model training, evaluation, visualisation, and coefficient interpretation.

## Objectives

- Explore the housing dataset using descriptive statistics and visualisations.
- Identify relevant features for predicting house prices.
- Handle missing values in numerical and categorical columns.
- Encode categorical variables using One-Hot Encoding.
- Analyse relationships between numerical features and sale prices.
- Train and evaluate a Linear Regression model.
- Visualise actual versus predicted prices and analyse residuals.
- Interpret model coefficients.
- Compare Linear Regression with Ridge Regression.

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## Dataset

**Dataset:** Ames Housing — House Prices: Advanced Regression Techniques

**Source:** https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data

Download the `train.csv` file from Kaggle and place it in the project directory.

The dataset contains housing characteristics and a `SalePrice` target column. This project uses selected features to predict the sale price of a house.

## Project Structure

```text
Task1-House-Price-Prediction/
├── train.csv
├── Task1_House_Price_Prediction.ipynb
├── README.md
└── output/
    ├── house_price_predictions.csv
    ├── model_comparison.csv
    └── linear_regression_coefficients.csv
```

## Project Workflow

### 1. Data Loading and Exploration
Load the dataset using Pandas and examine its dimensions, data types, descriptive statistics, duplicate records, and missing values.

### 2. Exploratory Data Analysis
Visualise the distribution of house sale prices using histograms and box plots. Use a correlation heatmap to examine relationships between numerical features and the target variable.

### 3. Feature Selection
Select relevant features representing house size, quality, age, facilities, and location. Use `SalePrice` as the target variable.

### 4. Data Preprocessing
- Impute missing numerical values using the median.
- Impute missing categorical values using the most frequent category.
- Apply One-Hot Encoding to categorical features.
- Use a Scikit-learn pipeline to keep preprocessing consistent and avoid data leakage.

### 5. Train-Test Split
Split the data into 80% training data and 20% testing data. The training data is used to fit the model, while the testing data evaluates its performance on unseen records.

### 6. Model Training
Train a Linear Regression model using Scikit-learn. Optionally, train a Ridge Regression model to compare the effect of regularisation.

### 7. Model Evaluation
Evaluate model performance using:

- **Mean Squared Error (MSE):** Measures the average squared prediction error.
- **Root Mean Squared Error (RMSE):** Measures prediction error on the same scale as the target price.
- **R² Score:** Measures model performance relative to predicting the mean target value.

### 8. Visualisation and Interpretation
- Actual versus predicted house prices scatter plot.
- Residual plot for analysing prediction errors.
- Correlation heatmap.
- Feature coefficient analysis.
- Performance comparison between Linear Regression and Ridge Regression.

## Installation

Install the required libraries:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```

## How to Run

1. Download `train.csv` from Kaggle.
2. Place `train.csv` in the project directory.
3. Open a terminal or command prompt in the project directory.
4. Start Jupyter Notebook:

```bash
jupyter notebook
```

5. Open `Task1_House_Price_Prediction.ipynb`.
6. Run the notebook cells in order.
7. Review the evaluation metrics, visualisations, and generated output files.

## Results

The notebook reports the MSE, RMSE, and R² score for the trained models. It also generates prediction records, coefficient information, and a comparison of Linear Regression and Ridge Regression.

Actual performance values depend on the dataset, selected features, and model settings. Record the results produced by your notebook rather than assuming predetermined scores.

## Applications

- Estimating residential property prices.
- Understanding relationships between housing characteristics and prices.
- Supporting preliminary real estate market analysis.
- Learning regression modelling and model evaluation.

## Conclusion

This project demonstrates how Linear Regression can be applied to house price prediction using a real-world housing dataset. Data preprocessing, feature selection, model evaluation, residual analysis, and coefficient interpretation help explain the model's performance and limitations. Ridge Regression provides an additional comparison to investigate whether regularisation improves predictive performance.

## References

- Kaggle Ames Housing Dataset: https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data
- Scikit-learn Linear Regression: https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html
- Scikit-learn Mean Squared Error: https://scikit-learn.org/stable/modules/generated/sklearn.metrics.mean_squared_error.html
- Scikit-learn R² Score: https://scikit-learn.org/stable/modules/generated/sklearn.metrics.r2_score.html
- Scikit-learn One-Hot Encoder: https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.OneHotEncoder.html
