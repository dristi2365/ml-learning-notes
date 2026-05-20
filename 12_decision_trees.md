# Decision Trees

A decision tree thinks exactly like a human making a decision —
it asks questions and follows the answers to reach a conclusion.

## Simple real life example:
Do I have to go somewhere today?
├── Yes → Shower immediately
└── No → Can I wait a few days?
          ├── Yes → Wait
          └── No → Shower anyway

## How it works in ML:
The model learns which questions to ask from training data
and in what order to best separate the classes.

## Key terms:
- Root node — the very first question at the top
- Branch — the yes/no path from each question
- Leaf node — the final answer at the bottom
- Depth — how many levels of questions the tree has

## Advantages:
- Very easy to understand and explain
- Works for both classification and regression
- No need to scale or normalize data

## Disadvantages:
- Can overfit easily if tree gets too deep
- Small changes in data can create very different trees
- Not the most accurate algorithm alone

## Overfitting in Decision Trees:
A tree that's too deep memorizes training data.
Solution: pruning — cutting off branches that don't add value.

## Real world examples:
- Medical diagnosis
- Loan approval decisions
- Customer churn prediction
