# Crop-Price-Prediction-
This project focuses on analyzing and predicting agricultural commodity prices, specifically for Wheat in Gujarat, India, by integrating market price data with weather information. The code performs data loading, cleaning, feature engineering, and preliminary analysis to understand the factors influencing commodity prices.
 Features

# Data Loading: 
Imports price and quantity data from CSV files (price_data.csv and quantity_data.csv) and weather data from weather_data.csv. 


# Data Preprocessing:

1.Fills missing values in min_price and max_price columns using linear interpolation. 

2.Converts date columns to datetime objects for proper merging and feature extraction. 

3.Data Merging: Combines price, quantity, and weather dataframes based on date and market_name to create a comprehensive dataset. 


# Feature Engineering:

1.Applies Label Encoding to district_name and market_name to convert categorical features into numerical labels. 

2.Extracts month and day_of_week from the date column. 


3.Categorizes months into seasons (Winter, Summer, Monsoon, Post-Monsoon). 

# Exploratory Data Analysis (EDA):

1.Generates relational plots to visualize the relationship between modal_price and district_labels across different seasons. 

2.Creates bar plots showing modal_price distribution per district. 

3.Analyzes modal_price trends based on day_of_week and season. 

# File Structure

price_data.csv: Contains historical price information for agricultural commodities. 

quantity_data.csv: Contains quantity data related to agricultural commodities. 

weather_data.csv: Contains weather parameters like temperature, dew, humidity, precipitation probability, and wind speed. 

(Note: price_data.csv, quantity_data.csv, and weather_data.csv are referenced in the code and are expected to be in the same directory as the script.)

# Installation
To run this code, you need to have the following Python libraries installed:

1.pandas 

2.numpy 

3.scikit-learn

4.seaborn 

5.plotly.express 

You can install them using pip:

pip install pandas numpy scikit-learn seaborn plotly-express
