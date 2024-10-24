# project-one
House Price Prediction and Analysis
Project Overview
This project focuses on predicting house prices across the United States using basic property features such as the number of bedrooms, bathrooms, and home type. The goal was to analyze the relationship between these features and house prices and determine how well a linear regression model could predict prices. We also explored geographic price variation by analyzing the median house prices by state and attempted to improve the model by applying logarithmic transformations and categorizing key features.

Objective: Build a linear regression model to predict house prices based on basic features.
           Assess the relationship between bedrooms, bathrooms, and home type with house prices.
           Analyze regional price variations by calculating the median house prices for each state.
           Evaluate the performance of different approaches, including normal linear regression, log transformations, and feature binning.

Dataset
The dataset is sourced from Zillow, a leading real estate marketplace, and includes detailed information on housing properties across the United States. 

Key variables include:
  price: The sale price of the house.
  bedrooms: Number of bedrooms in the house.
  bathrooms: Number of bathrooms in the house.
  homeType: Type of the house (e.g., single-family home, condo, townhouse).
  state, city: Geographic location of the house.

Modeling Approach

Data Cleaning: Removed rows with missing, zero, or infinite values for house prices.
Linear Regression: Built a simple linear regression model using bedrooms, bathrooms, and home type as the independent variables.
Logarithmic Transformation: Applied a log transformation to the target variable (price) to reduce skewness in price data.
Binning: Categorized bedrooms and bathrooms into bins to capture non-linear relationships between these features and house prices.
Geographic Analysis: Calculated and visualized the median house prices across different U.S. states.
Results
The R-squared value of the basic model was 0.26, meaning that only 26% of the variation in house prices was explained by the selected features.
Median house price by state analysis revealed significant geographic differences, with states like California and Hawaii having much higher median prices compared to states like Indiana and Nebraska.
The model struggled to predict high-end properties, as additional factors such as location, amenities, and property features were not included in the model.

Key Findings
Bedrooms, bathrooms, and home type are useful but insufficient predictors of house prices.
Location plays a significant role in price determination, and more granular location data would improve the model.
Logarithmic transformations and feature binning provided slight improvements but did not significantly enhance the model's performance.
Future models should incorporate more features and explore non-linear modeling techniques to capture price variability more effectively.
