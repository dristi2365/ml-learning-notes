# Random Forest

Random Forest builds hundreds of decision trees and makes 
them all vote on the answer. The majority vote wins.

## The problem with a single Decision Tree:
One tree can overfit — it makes very specific decisions 
based on training data that don't generalize well to new data.
Like asking one person for advice — they might be biased.

## Solution — ask many trees!
Build hundreds of different trees and take the majority vote.
Like asking 100 doctors for a diagnosis instead of just one.

## How it works:
1. Create many random subsets of training data
2. Build a decision tree for each subset
3. For a new data point, every tree makes a prediction
4. Final answer = majority vote of all trees

Example:
Tree 1 → Spam
Tree 2 → Spam
Tree 3 → Not Spam  → Majority says SPAM ✅
Tree 4 → Spam
Tree 5 → Spam

## The "Random" part:
Two sources of randomness make each tree different:
- Random data — each tree trains on a random subset of rows
- Random features — each tree only considers random features

## Why better than single Decision Tree:
- Reduces overfitting significantly
- More accurate — wisdom of many trees beats one tree
- More stable — small data changes don't affect result much

## Advantages:
- Very accurate general purpose algorithm
- Handles overfitting much better than single decision tree
- Works well without much data preparation

## Disadvantages:
- Slower than single decision tree
- Harder to interpret — can't draw 500 trees
- Uses more memory

## Bonus — Feature Importance:
Random Forest can tell you which features were most useful.
Example for spam classifier:
- Contains "free money" — 35% importance
- Number of links — 28% importance
- Contains "winner" — 20% importance

## Real world examples:
- Fraud detection in banking
- Disease prediction in healthcare
- Stock market prediction
