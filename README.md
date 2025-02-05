# Predicting Used Car Sale Prices

## Problem Description
In this project, we work with a comprehensive dataset containing information on vehicles and their listings at various dealerships. The dataset encompasses a wide range of attributes, from vehicle specifications to dealership details. Our objective is to extract valuable insights and knowledge from this data. We explore predictive modeling tasks, such as:

- Predicting vehicle prices
- Assessing the likelihood of accidents
- Estimating potential savings

Additionally, classification tasks, clustering, and geospatial analysis are used to understand dealership characteristics and vehicle distribution. This multifaceted dataset offers an opportunity to gain a deeper understanding of the automotive market and make informed decisions based on the provided information.

## Forecasting Problem
At the core of this project lies a critical forecasting problem: accurately predicting the prices of used cars. Vehicle price is a pivotal component of the automotive market, influenced by various factors such as:

- Brand, model, and year
- Mileage and condition
- Market trends

Developing a precise pricing model enables consumers to assess vehicle value, influencing trade decisions. Dealerships can use this model to set competitive prices and manage inventory. Financial institutions can employ these predictions for loan underwriting, while insurance companies can use them to evaluate vehicle value for policy underwriting and accident likelihood assessments.

## Types of Variables/Features
The dataset contains 39 variables, categorized into four types:

1. **Categorical Variables**:  
   Examples: `body_type`, `city`

2. **Numerical Attributes**:  
   Examples: `daysonmarket`, `horsepower`

3. **Boolean Variables**:  
   Examples: `franchise_dealer`, `has_accidents`

4. **Geospatial Data**:  
   Examples: `latitude`, `longitude`

These features can be further classified into vehicle-specific, sales-related, dealership, and geospatial data. This broad range of features offers a unique opportunity to enhance our understanding of the car market.

## Data Summary and Main Data Characteristics
- **Training Dataset**: 3,500 entries
- **Test Dataset**: 1,500 entries

The dataset contains both intrinsic car attributes (e.g., engine type, horsepower) and extrinsic factors (e.g., accident history, days on market). These variables provide valuable insights into the automotive market dynamics.

## Steps Involved in Developing the Model

### 1. Exploratory Data Analysis (EDA)
The dataset is analyzed to understand the distribution of features and identify relationships between features and vehicle prices. Key insights guide the preprocessing and modeling steps.

### 2. Data Preprocessing
- Missing values are identified and handled through removal or imputation.
- Categorical variables are encoded using techniques such as **one-hot encoding**.
- Numerical features are scaled if required to ensure optimal model performance.

### 3. Feature Selection and Engineering
- Relevant features with significant impacts on price prediction are selected.
- New features are created using **feature engineering techniques** like extracting or combining information from existing features.

### 4. Model Selection
Various regression models are considered for training, including:
- **XGBoost**
- **GradientBoostingRegressor**
- **DecisionTreeRegressor**

These models are trained on the preprocessed dataset, and their performance is evaluated using metrics such as **Root Mean Squared Error (RMSE)**.

### 5. Model Tuning
Hyperparameter tuning is performed using techniques like **GridSearchCV** to identify the best set of hyperparameters for each model. This step optimizes the model's performance.

### 6. Model Evaluation
The final models are evaluated to assess their performance in predicting used car prices. Metrics such as RMSE and cross-validation scores are used to determine the models' accuracy.

## Conclusion
The goal of this project is to provide accurate price predictions for used cars by using data preprocessing, feature engineering, model selection, and hyperparameter tuning. By following these steps, the most effective model is selected based on performance metrics.
