# Linear Regression

Used for regression problems — predicting a number.

## Simple example:
Predicting exam score based on hours studied.
More hours = higher score. Linear regression draws a 
straight line through the data representing this relationship.

## The formula:
y = mx + b
- y = prediction (exam score)
- x = input (hours studied)
- m = slope (steepness of line)
- b = intercept (where line crosses y axis)

## Multiple Linear Regression:
When you have more than one feature affecting the prediction.
Example: hours studied + hours of sleep + attendance → exam score

## When to use:
- Predicting a continuous number
- When relationship between input and output is roughly linear
- When you want a simple explainable model

## Limitations:
- Only works when relationship is actually linear
- Sensitive to outliers
- Can't capture complex patterns

## Real world examples:
- Predicting house prices based on size
- Predicting salary based on years of experience
- Predicting crop yield based on rainfall

## Important:
Cannot be used for classification problems like spam detection
because those require predicting a category, not a number.
