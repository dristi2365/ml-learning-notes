# Data Visualization

Turning numbers into charts so patterns become easy 
to see and understand.

## Simple analogy:
Reading 500,000 numbers vs looking at a bar chart —
the chart tells the story in seconds.

## Main library — Matplotlib:
```python
import matplotlib.pyplot as plt
```

## Chart types and when to use them:

| Situation | Chart Type |
|-----------|-----------|
| Comparing categories | Bar Chart |
| Trend over time | Line Chart |
| Parts of a whole | Pie Chart |
| Distribution of values | Histogram |
| Relationship between two variables | Scatter Plot |
| Spread and outliers | Box Plot |

## Bar Chart — comparing categories:
```python
plt.bar(categories, values, color="steelblue")
plt.title("Title")
plt.xlabel("X label")
plt.ylabel("Y label")
plt.show()
```
Example: grade distribution, sales by region.

## Line Chart — trends over time:
```python
plt.plot(years, values, marker="o", color="green")
plt.show()
```
Example: pass rates over years, stock prices over time.

## Pie Chart — parts of a whole:
```python
plt.pie(sizes, labels=labels, autopct="%1.1f%%")
plt.show()
```
Example: pass vs fail percentage, budget breakdown.

## Histogram — distribution of values:
```python
plt.hist(data, bins=20, color="purple", edgecolor="white")
plt.show()
```
Example: exam score distribution, age distribution.

## Scatter Plot — relationship between two variables:
```python
plt.scatter(x_values, y_values, color="red")
plt.show()
```
Example: study hours vs score, height vs weight.

## Box Plot — spread and outliers:
```python
plt.boxplot(data)
plt.show()
```
Example: salary distribution, test score spread.

## Essential settings:
```python
plt.title("Chart Title")
plt.xlabel("X axis label")
plt.ylabel("Y axis label")
plt.legend()
plt.tight_layout()
plt.savefig("chart.png", dpi=150)
plt.show()
plt.close()
```

## Seaborn — prettier charts with less code:
```python
import seaborn as sns
sns.barplot(x=categories, y=values)
sns.heatmap(df.corr(), annot=True)
```

## Quick rule:
- Comparing → Bar Chart
- Time trend → Line Chart
- Proportion → Pie Chart
- Distribution → Histogram
- Relationship → Scatter Plot
- Outliers → Box Plot
