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


## Model Evaluation and Results

We attempted to train above mentioned regression models to predict the prices of used cars.

### Hyperparameter Tuning and Feature Selection
Hyperparameter tuning was performed using **GridSearchCV** to find the optimal set of parameters for each model. Additionally, the top 10 features, as determined by their importance in the regression models, were selected for training.

### Model Performance
## Model Evaluation and Results

### XGBoost
Initially, our **XGBoost** model showed promise with an initial score of **6648**. After thorough data cleaning and refining the one-hot encoding process, its performance improved significantly. The refined model achieved a remarkable score of **5324**, highlighting the importance of data quality in machine learning. This improvement resulted in more accurate predictions and emphasized how effective data preprocessing is for enhancing model performance.

### GradientBoostingRegressor
At the outset, the **GradientBoostingRegressor** delivered a score of **5841**, demonstrating strong predictive capabilities. After extensive data cleaning and improvements to one-hot encoding, the model's performance saw a substantial boost. It achieved a commendable score of **4835**, further reinforcing its exceptional predictive power. This improvement underscores the importance of data preprocessing in optimizing model performance.

#### GradientBoostingRegressor's Superior Performance
- **Ensemble Learning Approach**:  
  The **GradientBoostingRegressor** utilizes an ensemble learning approach, which combines the predictions of multiple weak learners to create a robust and powerful model. This ensemble technique contributes to better predictive capabilities, making it a reliable choice for price prediction.
  
- **Strong Hyperparameter Tuning**:  
  The fine-tuning process significantly enhanced the model's performance. Key hyperparameters such as a **learning rate of 0.01**, **maximum depth of 12**, and **800 estimators** were selected to optimize the model for accuracy and reliability. This hyperparameter selection played a crucial role in improving the model's predictions.

- **Effective Feature Engineering**:  
  The improvement in data quality and refinement of one-hot encoding further boosted the **GradientBoostingRegressor**'s performance. This highlights the model's ability to leverage clean and well-prepared data for enhanced predictions.

- **Final Score of 4835**:  
  After these adjustments, the **GradientBoostingRegressor** achieved a final score of **4835**, signifying its remarkable predictive abilities. This score indicates the model's precision and its ability to make accurate predictions consistently.

### DecisionTreeRegressor
The **DecisionTreeRegressor**, initially scoring **8986**, underwent a similar transformation after data cleaning and refining the one-hot encoding. The model's predictive power surged, and it achieved an impressive score of **7075**. However, the journey from a higher initial score to a lower final score underscores the importance of data quality and feature engineering in model refinement. Although the **DecisionTreeRegressor** showed improvement, it still lagged behind the other models in terms of predictive performance.

### Conclusion: GradientBoostingRegressor as the Top-Performing Model
The choice of **GradientBoostingRegressor** as the top-performing model is supported by several key factors:

- **Ensemble Learning**: The combination of multiple weak learners improves prediction accuracy.
- **Hyperparameter Tuning**: Careful optimization of hyperparameters played a significant role in boosting model performance.
- **Feature Engineering**: Effective data preprocessing, such as one-hot encoding and outlier removal, contributed to the model's precision.

The final score of **4835** solidifies **GradientBoostingRegressor** as the most reliable model for accurately predicting used car prices, making it the optimal choice for our project.

