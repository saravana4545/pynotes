---
title: Numpy-Using-Pandas
date: 2024-12-21
author: Your Name
cell_count: 35
score: 35
---

```python
# Handling Missing Data
```


```python
#import neccessary libraries
```


```python
import pandas as pd
```


```python
import numpy as np
```


```python
# Create a DataFrame with missing values
```


```python
#np.nan: Represents missing values.
```


```python

```


```python
data = {
    'Name': ['Alice', 'Bob', None],
    'Age': [25, np.nan, 35],
    'City': ['New York', None, 'Chicago']
}
```


```python
df = pd.DataFrame(data)
```


```python
# Fill missing values with 'Unknown' or 0
```


```python
#df.fillna(): Replaces missing values with specified values.
```


```python
df_filled = df.fillna({'Name': 'Unknown', 'Age': 0, 'City': 'Unknown'})
```


```python
#print the variable
```


```python
print(df_filled)
```

          Name   Age      City
    0    Alice  25.0  New York
    1      Bob   0.0   Unknown
    2  Unknown  35.0   Chicago



```python

```


```python

```


```python
# Sort by Age in descending order
```


```python
sorted_df = df.sort_values(by='Age', ascending=False)
```


```python
print(sorted_df)
```

        Name   Age      City
    2   None  35.0   Chicago
    0  Alice  25.0  New York
    1    Bob   NaN      None



```python

```


```python
# Group by 'City' and calculate the average Age
```


```python
grouped_df = df.groupby('City')['Age'].mean()
```


```python
print(grouped_df)
```

    City
    Chicago     35.0
    New York    25.0
    Name: Age, dtype: float64



```python

```


```python
# Summary statistics
```


```python
print(df.describe())
```

                 Age
    count   2.000000
    mean   30.000000
    std     7.071068
    min    25.000000
    25%    27.500000
    50%    30.000000
    75%    32.500000
    max    35.000000



```python

```


```python
# Merging DataFrames
```


```python
df1 = pd.DataFrame({'ID': [1, 2, 3], 'Name': ['Alice', 'Bob', 'Charlie']})
```


```python
df2 = pd.DataFrame({'ID': [1, 2, 4], 'Score': [85, 90, 95]})
```


```python
# Merge on the 'ID' column
```


```python
merged_df = pd.merge(df1, df2, on='ID', how='inner')
```


```python
print(merged_df)
```

       ID   Name  Score
    0   1  Alice     85
    1   2    Bob     90



```python

```


```python

```


---
**Score: 35**
