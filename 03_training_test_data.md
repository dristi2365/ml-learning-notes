# Training Data vs Test Data

When building a ML model you can't use all your data for training.

## Why?
If you study only the exact exam questions, you'll ace that exam 
but fail a different one on the same topic. You memorized, not learned.
ML has the same problem.

## Solution — Split the data:

**Training data (80%):**
What the model learns from. Like study material before an exam.

**Test data (20%):**
Data the model has never seen. Used to check if it actually learned.
Like the real exam.

## Three way split (more advanced):
- Training data (60-70%) — model learns from this
- Validation data (10-20%) — used during training to tune the model
- Test data (20%) — final check at the very end

## Simple rule:
- Training = learning
- Test = checking
