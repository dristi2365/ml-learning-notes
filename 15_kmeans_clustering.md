# K-Means Clustering

K-Means is an unsupervised learning algorithm — no labels needed.
It finds natural groups in data on its own.

## Simple analogy:
Like sorting a mixed bag of fruits into groups without being 
told what the groups are — you just naturally group 
similar ones together.

## How it works:
1. Choose K — decide how many clusters you want
2. Place K random centroids (center points) in the data
3. Assign each point to the nearest centroid
4. Recalculate the center of each group
5. Repeat until nothing changes

## Choosing the right K — Elbow Method:
Try different values of K and plot results.
The point where improvement slows down looks like an elbow
— that's your best K value.

## Key difference from KNN:
| | KNN | K-Means |
|--|--|--|
| Type | Supervised | Unsupervised |
| Purpose | Classification | Clustering |
| K means | Number of neighbors | Number of clusters |
| Labels | Required | Not required |

Despite similar names they are completely different algorithms!

## Advantages:
- Simple and fast
- Scales well to large datasets

## Disadvantages:
- Must choose K in advance
- Sensitive to outliers
- Only finds circular shaped clusters
- Results vary since centroids start randomly

## Real world examples:
- Customer segmentation
- Document clustering
- Image compression
- Anomaly detection

