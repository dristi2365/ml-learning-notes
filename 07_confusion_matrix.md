# Confusion Matrix, Accuracy, Precision, Recall

A confusion matrix shows how well your classification model 
performed — not just overall accuracy but where it went wrong.

## Example — Spam Classifier (100 emails):

|                    | Predicted Spam | Predicted Not Spam |
|--------------------|----------------|--------------------|
| Actual Spam        | 45 (TP)        | 5 (FN)             |
| Actual Not Spam    | 8 (FP)         | 42 (TN)            |

## The four values:
- True Positive (TP) = predicted yes, actually yes ✅
- True Negative (TN) = predicted no, actually no ✅
- False Positive (FP) = predicted yes, actually no ❌
- False Negative (FN) = predicted no, actually yes ❌

Easy way to remember:
- True = model was right
- False = model was wrong
- Positive = model predicted yes
- Negative = model predicted no

## Three metrics:

**Accuracy** = (TP + TN) / Total
How many predictions were correct overall?

**Precision** = TP / (TP + FP)
Out of all positive predictions, how many were actually positive?
High precision = fewer false alarms

**Recall** = TP / (TP + FN)
Out of all actual positives, how many did we catch?
High recall = fewer missed cases

## Which matters more?

**Spam filter** → Precision matters more
Don't want to accidentally delete a legitimate important email.

**Cancer detection** → Recall matters more
Don't want to miss a real cancer case even if it means 
some false alarms. A missed cancer could cost someone 
their life. A false alarm just means more tests.
