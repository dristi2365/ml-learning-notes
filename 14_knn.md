# K-Nearest Neighbors (KNN)

KNN is one of the simplest ML algorithms. It doesn't learn 
during training — it just memorizes data and makes decisions 
based on similarity.

## Simple analogy:
"Tell me who your neighbors are and I'll tell you who you are."
Like judging if an area is safe by looking at the people 
living closest to it.

## How it works:
1. Store all training data points
2. When a new point comes in, find the K closest points
3. Look at what class those K neighbors belong to
4. Majority vote wins — assign that class to the new point

## What is K?
K is the number of neighbors you look at.
- K=1 → look at just the 1 closest neighbor
- K=3 → look at 3 closest, majority wins
- Too small K → overfitting
- Too large K → underfitting
- Usually use an odd number to avoid ties

## How does it measure distance?
Euclidean distance — straight line distance between two points.
distance = √((x2-x1)² + (y2-y1)²)
Same formula used in the padel project for total_movement!

## Advantages:
- Very simple to understand and implement
- No training time — just stores data
- Works well for small datasets

## Disadvantages:
- Slow at prediction — calculates distance to every point
- Struggles with large datasets
- Features need to be normalized

## Real world examples:
- Movie recommendation systems
- Medical diagnosis
- Handwriting recognition

