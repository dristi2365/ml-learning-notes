# Overfitting and Underfitting

## Overfitting
When the model memorizes the training data instead of 
learning general patterns.

Like a student who memorizes exact practice questions 
without understanding the topic — aces practice exams 
but fails the real exam.

Signs:
- Very high accuracy on training data
- Very low accuracy on test data
- Big gap between the two

## Underfitting
When the model hasn't learned enough from the training data.
Performs badly on both training AND test data.

Like a student who barely studied — fails both practice 
exams and the real exam.

Signs:
- Low accuracy on both training AND test data
- Model is too simple for the problem

## The Sweet Spot
A model that learns general patterns and performs well 
on new unseen data. Not too complex, not too simple.

Underfitting → Sweet Spot → Overfitting
barely learned → learned well → memorized
bad on both → good on both → great on train, bad on test
