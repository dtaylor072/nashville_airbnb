# Predicting the Prices of Airbnb Rentals in Nashville, Tennessee
### Economic Question:
As the sharing economy has become a larger part of the global economy in recent years, there has been a sharp increase in the number and variety of properties available for rent on platforms such as Airbnb. Nashville, being a popular destination for tourists, has seen many of its properties converted to Airbnb rentals to satisfy tourist demand. These rental properties vary widely in value based on hundreds of factors such as location, size, number of bedrooms, and “host” reputation. The purpose of this project is to determine the factors that play the largest roles in determining the nightly rental price for an Airbnb listing in Nashville.
### Data Source:
The data was downloaded from [InsideAirbnb.com](InsideAirbnb.com), an independent platform which scrapes listing data from Airbnb.com on regular intervals to provide information to the public that Airbnb not directly provide. The data used in this analysis was scraped in September of 2019 and was requested to inform public debate and guide policymaking with regards to short-term rental properties in Nashville. Check out [this article](https://www.bloomberg.com/news/articles/2019-05-23/meet-murray-cox-airbnb-s-public-enemy-no-1-in-new-york) on Murray Cox, the creator and owner of InsideAirbnb.com, to learn more about why this data is important.
### Data Description:
The dataset has a total of n=4958 observations (distinct listings on Airbnb) in p=60 variables. The dataset was cleaned to remove observations with missing feature values and features with a high number of missing observations. The features for each listing relate to the nature of the property (e.g., number of bedroom and bathrooms, square feet, location) as well as the host who has listed the property (e.g., number of reviews, listings, and ratings). The response variable in this analysis is ‘price’, which denotes the price charged by a host on Airbnb for one night’s stay at their listed property. This price excludes any additional fees that a guest might pay for their stay.
### Methodologies:
I will first fit a simple linear model to the data, and then move to regularized Ridge and LASSO models to help minimize the effects of non-explanatory features. I will then fit tree-based models, Random Forest and XGBoost (Extreme Gradient Boosting). XGBoost, combines both L1 and L2 regularization in a gradient-boosted decision trees (GBDT) model, allowing it to achieve high accuracy and efficiency without overfitting the training set. I will then analyze the parameters of the best model to determine the most important factors in determining the price of an Airbnb listing in Nashville.
### Expected Results:
I expect that the most important factors in determining the price of a listing are: the number of bedrooms and bathrooms, proximity to downtown Nashville, and number of host reviews. However, I estimate that the best model will not perform extremely well, because property values are influenced by many external factors and it is likely that the price variance cannot be captured solely with the data provided.
