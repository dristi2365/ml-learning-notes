# Correlation

Correlation measures how two variables relate — when one 
changes, does the other tend to change too?

## Correlation coefficient: -1 to +1

**+1 — Perfect positive correlation**
Both increase together. Example: hours studied and exam score.

**0 — No correlation**
No relationship. Example: shoe size and sleep hours.

**-1 — Perfect negative correlation**
One increases, other decreases. Example: price and quantity sold.

```python
df.corr()   # correlation matrix
```

## CRITICAL: Correlation does NOT mean Causation

Just because two things move together doesn't mean one 
causes the other.

Classic example: Ice cream sales and drowning deaths are 
correlated - both rise in summer. Ice cream doesn't cause 
drowning. Hidden factor (confounding variable): hot weather 
causes both more swimming and more ice cream eating.

## Heatmap visualization:
```python
import seaborn as sns
sns.heatmap(df.corr(), annot=True, cmap="coolwarm")
plt.show()
```

## Real world examples:
- Height and weight - positively correlated
- Temperature and heating costs - negatively correlated
- Study hours and grades - positively correlated
- Advertising spend and sales - correlated but not always causal
