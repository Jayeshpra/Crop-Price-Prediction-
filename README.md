# Crop-Price-Prediction-
This project focuses on analyzing and predicting agricultural commodity prices, specifically for Wheat in Gujarat, India, by integrating market price data with weather information. The code performs data loading, cleaning, feature engineering, and preliminary analysis to understand the factors influencing commodity prices.
 Features

Data Loading: Imports price and quantity data from CSV files (price_data.csv and quantity_data.csv) and weather data from weather_data.csv. 


Data Preprocessing:

Fills missing values in 

min_price and max_price columns using linear interpolation. 

Converts date columns to datetime objects for proper merging and feature extraction. 




Data Merging: Combines price, quantity, and weather dataframes based on date and market_name to create a comprehensive dataset. 


Feature Engineering:

Applies Label Encoding to 

district_name and market_name to convert categorical features into numerical labels. 

Extracts 

month and day_of_week from the date column. 


Categorizes months into 

seasons (Winter, Summer, Monsoon, Post-Monsoon). 

Exploratory Data Analysis (EDA):

Generates relational plots to visualize the relationship between 

modal_price and district_labels across different seasons. 

Creates bar plots showing 

modal_price distribution per district. 

Analyzes 

modal_price trends based on day_of_week and season. 

📂 File Structure


price_data.csv: Contains historical price information for agricultural commodities. 


quantity_data.csv: Contains quantity data related to agricultural commodities. 


weather_data.csv: Contains weather parameters like temperature, dew, humidity, precipitation probability, and wind speed. 

(Note: price_data.csv, quantity_data.csv, and weather_data.csv are referenced in the code and are expected to be in the same directory as the script.)

🛠️ Installation
To run this code, you need to have the following Python libraries installed:


pandas 


numpy 


scikit-learn (for LabelEncoder) 


seaborn 


plotly.express 

You can install them using pip:

Bash

pip install pandas numpy scikit-learn seaborn plotly-express
