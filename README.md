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

 # EDA 

The data visualization is performed using mainly seaborn & matplotlib library. For visualization, the following charts are used:

Count plot

Distplot

Histplot

Line chart

Scatter plot

Box plot

Correlation Heatmap

Pair Plot
