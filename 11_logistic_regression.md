# Logistic Regression

Despite the name, logistic regression is used for CLASSIFICATION not regression.

## Why not use Linear Regression for classification?
Linear regression predicts any number — including values like 1.3 or -0.4 
which make no sense for classification. We need values between 0 and 1.

## What Logistic Regression does:
Uses an S-shaped sigmoid curve that squeezes any input into a value 
between 0 and 1 — interpreted as a probability.

Example — predicting pass/fail:
- 1 hour studied → 0.10 (10% chance of passing) → Fail
- 5 hours studied → 0.75 (75% chance) → Pass
- 7 hours studied → 0.95 (95% chance) → Pass

Threshold is usually 0.5:
- Above 0.5 → one class
- Below 0.5 → other class

## When to use:
- Binary classification (spam/not spam, pass/fail, yes/no)
- When you want probabilities not just categories
- Simple fast baseline model

## Key difference:
| | Linear Regression | Logistic Regression |
|--|--|--|
| Output | Any number | Between 0 and 1 |
| Used for | Regression | Classification |
| Shape | Straight line | S-shaped curve |
