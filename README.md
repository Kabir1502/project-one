# project-one
Project One for Data Bootcamp via Columbia

Method of Analysis
In this analysis, we used linear regression to model the relationship between house prices and several key features: the number of bedrooms, bathrooms, and home type (using dummy variables for different home categories). The dataset was preprocessed to remove houses with missing, infinite, or zero price values to ensure data integrity.
The model was trained using the least-squares method, where the coefficients for each feature were estimated by minimizing the difference between the actual house prices and the predicted prices. The model included an intercept term to account for baseline variations in prices.

Why is the model struggling to predict higher-cost houses?

Our data set originally came with a whopping 118 columns, including factors such as rental leads, tax-assessed values, and types of property management. 
We tried to limit factors to apply our analysis, using the ordinary least squares method which requires linear variables (meaning they have a low correlation and are largely independent).
Given these constraints, we limited our data to bedrooms, bathrooms, and hometypes. While we originally tried to include factors such as the living area and the year the house was built, these factors showed a heavy correlation (living area with bedrooms and bathrooms, and year built with all three), resulting in huge errors in our calculations. 
While these factors are important, they may not capture all the nuances affecting higher-value homes' prices. Features such as location (specific neighborhoods), square footage (living area), recent renovations, amenities, or proximity to services can significantly impact prices, particularly in luxury markets.
