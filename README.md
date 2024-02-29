# Capstone Regression Project - Yes Bank Stock Closing Price Prediction

# Introduction 

We are provided with a Yes Bank dataset, a leading institution in the Indian financial sector, garnered attention following the 2018 fraud case involving its former CEO, Rana Kapoor. The main objective is to predict the stock’s closing price of the month.

# Problem Statement

Yes Bank, a prominent institution in the Indian financial sector, gained notoriety following the 2018 fraud case involving its former CEO, Rana Kapoor. This dataset encompasses monthly stock prices of Yes Bank since its establishment, encompassing metrics such as closing, opening, highest, and lowest prices for each month. The focal point revolves around discerning how such high-profile events, like the aforementioned scandal, have influenced the company's stock prices. Can time series models, or other predictive methodologies, effectively capture and predict the fluctuations resulting from such circumstances? The primary goal is to forecast the monthly closing price of Yes Bank's stock, leveraging insights gained from this analysis.

# Dataset Information

The given dataset contains the monthly stock prices of Yes Bank since its establishment and includes closing, opening, highest, and lowest prices for each month. The primary goal is to forecast the monthly closing price of the stock. The dataset has 185 rows and 5 columns. The dataset contains 0 missing/null values and 0 duplicate values.

The variables are described as follows:

**Date**       **:**  Date of the stock price record

**Open**       **:**  Opening price of the stock

**High**       **:**  Highest price of the stock for the day

**Low**        **:**  Lowest price of the stock for the day

**Close**      **:**  Closing price of the stock for the day

# Data Cleaning and Manipulation 

1.Handling Null & Duplicate Values

* The given dataset contains no null and duplicate values.

2.Converting Datatypes

* Converted column Date to datetime data type.

 # Exploratory Data Analysis 

The data visualization is performed using mainly seaborn & matplotlib library. For visualization, the following charts are used:

Count plot

Distplot

Histplot

Line chart

Scatter plot

Box plot

Correlation Heatmap

Pair Plot

# Prediction Models

To predict the stock's closing price, the four models were developed : Linear Regression, Lasso Regression, Ridge Regression and Random Forest. 'Open', 'High', and 'Low' features were aggregated by taking their mean and engineered additional features using lag values to capture temporal trends and patterns, including potential effects of the fraud case. These models were evaluated using various metrics to gain insights into the data, facilitating better decision-making for improved outcomes. 

1. Linear Regression:

A linear regression model is a statistical method used to model the relationship between one or more independent variables (predictors) and a dependent variable (outcome). It assumes a linear relationship between the predictors and the outcome, where the outcome variable is a linear combination of the predictor variables, with each predictor weighted by a coefficient.

2. Lasso Regression:

Lasso regression, short for Least Absolute Shrinkage and Selection Operator, is a regression technique that performs both variable selection and regularization to improve the predictive performance and interpretability of the model.

3. Ridge Regression:

Ridge Regression, also known as L2 Regularization, is a linear regression technique that incorporates regularization to prevent overfitting and improve the generalization of the model.

4. Random Forest:

Random Forest Regression is a machine learning technique that utilizes an ensemble of decision trees to make predictions. It's well-suited for regression tasks and offers advantages such as handling non-linear relationships and interactions between features, as well as being robust to overfitting and capable of handling large datasets with high dimensionality.

# Evaluation Metrics

Evaluation metrics are quantitative measures used to assess the performance of a machine learning model. These metrics provide insights into how well the model is performing and can help determine if the model is suitable for its intended task. Some common evaluation metrics for regression tasks include:

Mean Absolute Error (MAE): The average of the absolute differences between the predicted and actual values. It provides a measure of the average magnitude of errors in the predictions.

Mean Squared Error (MSE): The average of the squared differences between the predicted and actual values. It penalizes larger errors more heavily than MAE.

Root Mean Squared Error (RMSE): The square root of the MSE. It provides an interpretable measure of the average magnitude of errors in the same units as the target variable.

R-squared (R2) Score: A measure of how well the model fits the data, indicating the proportion of variance in the target variable that is explained by the model. It ranges from 0 to 1, with higher values indicating a better fit.

Adjusted R-squared: A variant of R2 that adjusts for the number of predictors in the model. It penalizes the inclusion of additional predictors that do not significantly improve the model fit.

# Conclusion

The primary goal is to forecast the monthly closing price of Yes Bank's stock, considering the impact of the 2018 fraud case, using historical monthly stock price data. The dataset includes metrics such as opening, closing, highest, and lowest prices for each month since the establishment of Yes Bank.

Due to fluctuations over time, especially significant events like the 2018 fraud, variables like 'Close' and 'Open', 'High', 'Low' may exhibit positive skewness. Applying log transformation has led to a more symmetrical distribution, improving the accuracy of predictions. The closing price shows high correlation with other variables.

The log transformation effectively reduced outliers in the dataset, contributing to a more robust model. However, completely removing outliers from a small dataset is generally not advisable.

I aggregated 'Open', 'High', and 'Low' features by taking their mean and engineered additional features using lag values to capture temporal trends and patterns, including potential effects of the fraud case.

Four machine learning models were constructed - Linear Regression, Lasso Regression, Ridge Regression, and Random Forest. Evaluation metrics provide insights into data, aiding decision-making for better outcomes. Cross-validation was utilized to estimate optimal values, ensuring robust and generalizable models for new data.

SHAP (SHapley Additive exPlanations) is an advanced method for studying model explainability in machine learning. It calculates the contribution of each feature to the final prediction, providing insights into how individual components of the model influence the overall outcome.

Given the dataset and features, our model demonstrates strong performance across all data points, showcasing its robustness in capturing patterns and trends within the data. This indicates that the model effectively generalizes to unseen instances and maintains consistent accuracy in its predictions. Such reliability underscores the efficacy of our model in addressing the complexities inherent in the dataset, thereby instilling confidence in its predictive capabilities.
