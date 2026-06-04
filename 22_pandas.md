# Pandas

Pandas is the most important Python library for data analysis.
Think of it as a super powerful Excel inside Python.

## Two main data structures:

**Series — 1 dimensional (single column)**
Just a list of values with an index.

**DataFrame — 2 dimensional (full table)**
Rows and columns — exactly like a spreadsheet.
Most of the time you will work with DataFrames.

## Creating a DataFrame:

From a dictionary:
```python
import pandas as pd
data = {
    "Name": ["Alice", "Bob", "Dristi"],
    "Age": [20, 22, 21],
    "Score": [85, 90, 95]
}
df = pd.DataFrame(data)
```

From a CSV file:
```python
df = pd.read_csv("data.csv")
```

## Most important operations:

**Reading data:**
```python
df = pd.read_csv("file.csv")
df = pd.read_excel("file.xlsx")
```

**Exploring data:**
```python
df.head()       # first 5 rows
df.tail()       # last 5 rows
df.shape        # (rows, columns)
df.info()       # data types and missing values
df.describe()   # basic statistics
```

**Selecting data:**
```python
df["Name"]              # one column
df[["Name", "Age"]]     # multiple columns
df.iloc[0]              # first row by position
```

**Filtering data:**
```python
df[df["Age"] > 21]      # rows where age above 21
df[df["Score"] > 80]    # rows where score above 80
```

**Handling missing values:**
```python
df.isnull().sum()   # count missing values
df.dropna()         # remove rows with missing values
df.fillna(0)        # fill missing values with 0
```

**Grouping and aggregating:**
```python
df.groupby("Age")["Score"].mean()   # average score by age
df["Grade"].value_counts()           # count by category
```

**Saving data:**
```python
df.to_csv("output.csv", index=False)
```

## Advantages:
- Makes data manipulation incredibly easy
- Handles large datasets efficiently
- Industry standard for data analysis in Python
- Works seamlessly with Matplotlib for visualization

## Real world uses:
- Loading and cleaning messy datasets
- Analyzing sales, financial or survey data
- Preparing data for ML models
- Generating reports and summaries
