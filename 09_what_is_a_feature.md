# What is a Feature?

A feature is an input variable — a piece of information 
you give to the model to help it make predictions.

## Example — Predicting rain:
- Temperature
- Humidity
- Cloud cover
- Wind speed
Each of these is a feature. Together they help the model 
predict whether it will rain or not.

## Example — Spam Classifier:
- Number of exclamation marks
- Presence of words like "free", "winner"
- Length of email
- Number of links

## Example — Predicting house price:
- Size of the house
- Number of bedrooms
- Location
- Age of the building
All inputs that help predict the final price.

## Feature Engineering:
Sometimes raw data isn't directly useful — you create 
better features from it.

Example: You have a taxi pickup location and dropoff 
location as coordinates. Instead of using raw coordinates 
as features, you calculate the distance between them. 
That calculated distance is a much more useful feature 
for predicting fare price.

Better features = better model.
Even a simple model with great features can outperform 
a complex model with poor features.
