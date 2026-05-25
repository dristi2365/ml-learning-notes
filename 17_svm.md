# Support Vector Machine (SVM)

SVM finds the best line to separate two classes — 
the one with the maximum gap between the groups.

## Simple analogy:
Imagine red and blue dots on paper. Many lines could 
separate them. SVM finds the line with the widest 
gap between the two groups.

## Key concepts:

**Hyperplane** — the line/plane that separates the classes.
In 2D it's a line, in higher dimensions it's a hyperplane.

**Support Vectors** — the data points closest to the 
hyperplane on each side. They define where the hyperplane goes.

**Margin** — the gap between the hyperplane and the nearest 
points on each side. SVM maximizes this margin.
Wider margin = more confident decisions.

## What if data isn't linearly separable?
SVM uses the Kernel Trick — transforms data into a higher 
dimension where it becomes separable.

Analogy: Red and blue marbles mixed on a table can't be 
separated with a straight line. But tilt the table and 
they roll apart naturally. That's the kernel trick — 
changing perspective to make separation possible.

## Advantages:
- Very effective in high dimensional spaces
- Memory efficient — only uses support vectors
- Very accurate for classification

## Disadvantages:
- Slow on very large datasets
- Sensitive to feature scaling
- Hard to interpret
- Choosing the right kernel can be tricky

## SVM vs Logistic Regression:
- Logistic Regression gives probabilities
- SVM finds maximum margin boundary
- SVM generally performs better on complex datasets
- Logistic Regression is easier to interpret

## Real world examples:
- Image classification
- Text categorization
- Medical diagnosis
- Face detection
