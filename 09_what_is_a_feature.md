# What is a Feature?

A feature is an input variable — a piece of information 
you give to the model to help it make predictions.

## Example — Predicting rain:
- Temperature
- Humidity
- Cloud cover
- Wind speed
Each of these is a feature.

## Example — Spam Classifier:
- Number of exclamation marks
- Presence of words like "free", "winner"
- Length of email
- Number of links

## Feature Engineering:
Sometimes you create better features from raw data.
Example: from pickup/dropoff coordinates → calculate distance.
Better features = better model.

## From the Padel Project:
Features used for shot classification:
- Previous position of player (prev_x, prev_y)
- Current position (center_x, center_y)
- dx — horizontal movement
- dy — vertical movement
- total_movement — overall movement magnitude
