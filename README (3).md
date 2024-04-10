
# HOUSING DATA ANALYSIS

Delve into the King County House sales dataset, a comprehensive repository of housing sales information in King County, USA.
Our aim is to provide precise insights to assist homeowners and real estate agencies in making informed decisions regarding property valuation and understanding market trends.



## Business understanding
In King County's real estate scene, stakeholders encounter difficulties grasping what drives property values and market shifts. This research aims to tackle these hurdles by examining how property attributes, location factors, market preferences, and time trends interact. By understanding these elements better, stakeholders can make smarter choices on property investments, pricing tactics, and market strategies, empowering them to thrive in King County's dynamic real estate landscape.






## Objectives
1. Identify the key factors influencing housing prices based on historical data.
2. Quantify the impact of these factors on the buying and selling prices of houses.
3. Develop predictive models to forecast housing prices accurately.
4. Provide actionable recommendations to stakeholders based on the analysis to enhance their decision-making processes in the real estate market
## Modelling
The Baseline model initially employed two simple linear regression models to showcase the correlation between price and two highly correlated variables: sqft_living and bathrooms.

Subsequently, we delved into crafting multiple linear regression models and iteratively refining them through feature selection.

Our process included feature selection and the development of a polynomial regression model, followed by validation using cross-validation techniques.

## Results
Our polynomial regression model is preferred as it achieved the highest R-squared value of 0.58, surpassing both the multiple linear regression model (0.53) and the simple regression analyses (0.41 and 0.29)

The features below impact price such that an increase will cause an increase in the price of the property:
'sqft_living' , 'bathrooms' , 'sqft_above' ,  'sqft_basement' and 'waterfront'

On the other hand 'yr_built' , 'bedrooms' and 'sqft_lot" has a negative impact on price shown by its negatice coefficient
## Limitations
1. The dataset may lack additional property-specific characteristics that could provide further insights into housing prices.

2. Multicollinearity: The existence of correlated predictors within the dataset can result in multicollinearity problems, complicating the accurate interpretation of the individual impacts of each feature.

3. Overfitting: Polynomial regression models are prone to overfitting. This is where the model tightly conforms to the training data but may struggle to perform well on new, unseen data. Overall the model was the best fit model for this prediction
## Recommendations
1. Further Data Collection: the dataset could be expanded to include additional property-specific characteristics that may influence housing prices, such as proximity to amenities and neighborhood demographics, and property condition. This can provide a more comprehensive understanding of the housing market dynamics.

2. Guard Against Overfitting: To mitigate the risk of overfitting in polynomial regression models, using techniques such as cross-validation, regularization could be considered, or reducing the complexity of the model by selecting an appropriate degree for the polynomial features.

3. Continuous Model Monitoring: Continuously monitoring the model's performance and validity over time as new data becomes available or market conditions change. Regular updates and recalibration may be necessary to ensure the model remains relevant and accurate.
## Conclusion

Based on our analysis, we have uncovered several significant insights into the factors influencing housing prices. Firstly, features such as waterfront views, larger living spaces (both above ground and in the basement), and certain construction attributes positively impact housing prices. Conversely, newer properties tend to command lower prices compared to older ones, and factors like the number of bedrooms and lot size are associated with decreased prices.