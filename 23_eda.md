# Exploratory Data Analysis (EDA)

EDA is the first step when you get a new dataset.
Before building any model — explore and understand the data.

## Simple analogy:
Like moving into a new house — before arranging furniture
you walk through every room and understand what you have.
EDA is walking through your data before making decisions.

## Why EDA is important:
- Understand the structure of your data
- Find missing values before they cause problems
- Spot outliers that could skew results
- Find patterns and relationships between variables
- Decide which features are useful for modeling
- Catch data quality issues early

## EDA process step by step:

**Step 1 — Load and preview:**
```python
df.head()      # first 5 rows
df.tail()      # last 5 rows
df.shape       # rows and columns
df.columns     # column names
```

**Step 2 — Understand data types:**
```python
df.info()      # data types and non-null counts
```

**Step 3 — Basic statistics:**
```python
df.describe()  # count, mean, min, max, std
```

**Step 4 — Check missing values:**
```python
df.isnull().sum()    # count missing per column
df.isnull().sum() / len(df) * 100  # percentage missing
```

**Step 5 — Check duplicates:**
```python
df.duplicated().sum()   # count duplicates
df.drop_duplicates()    # remove duplicates
```

**Step 6 — Value distributions:**
```python
df["column"].value_counts()   # frequency of each value
df["column"].unique()         # unique values
df["column"].nunique()        # number of unique values
```

**Step 7 — Correlations:**
```python
df.corr()   # correlation between numerical columns
```

**Step 8 — Visualize:**
Histograms, bar charts, scatter plots, box plots.

## What are outliers?
Data points very different from the rest.
Example: scores of 45, 50, 55, 60, 98 — 98 is an outlier.
Can be genuine or data entry errors.
Can skew averages and model results.

## What are missing values?
Empty cells in your dataset — data not collected or recorded.
Options: drop the row, fill with average, or fill with 0.

## Questions EDA answers:
- How many rows and columns do I have?
- What data types are there?
- Are there missing values or duplicates?
- What does the distribution look like?
- Are there outliers?
- Are there relationships between variables?
