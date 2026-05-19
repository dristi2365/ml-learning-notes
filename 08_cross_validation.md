# Cross Validation

## The problem with simple train/test split:
If by bad luck your 20% test data happens to be really easy 
or really hard, your accuracy score might not reflect how 
the model actually performs in real life.

## Solution — K-Fold Cross Validation:
Test the model multiple times on different parts of the data.

## How 5-Fold Cross Validation works:

Step 1 — Split data into 5 equal parts (folds):
Fold 1 | Fold 2 | Fold 3 | Fold 4 | Fold 5

Step 2 — Train and test 5 times:
Round 1: Train on 2,3,4,5 → Test on 1
Round 2: Train on 1,3,4,5 → Test on 2
Round 3: Train on 1,2,4,5 → Test on 3
Round 4: Train on 1,2,3,5 → Test on 4
Round 5: Train on 1,2,3,4 → Test on 5

Step 3 — Average the 5 accuracy scores

## Why is it better?
Every single data point gets used for both training AND 
testing at some point. Much more reliable than one single test.

## Simple analogy:
Instead of one exam to judge a student, give them 5 different 
exams and average the scores. Fairer and more accurate.

## When to use it?
When you have limited data and can't afford to waste 20% 
just for testing.
