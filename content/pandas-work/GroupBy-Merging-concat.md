---
title: Groupby-Merging-Concat
date: 2024-12-08
author: Your Name
cell_count: 17
score: 15
---

```python
#import pandas library
```


```python
import pandas as pd
```


```python
# GroupBy and Aggregations
```


```python
data = {
    'Department': ['HR', 'IT', 'HR', 'IT', 'Finance'],
    'Salary': [50000, 60000, 45000, 70000, 65000]
}

```


```python
df = pd.DataFrame(data)
```


```python
# Grouping and aggregating
```


```python
grouped = df.groupby('Department')['Salary'].agg(['mean', 'sum', 'max'])
print(grouped)
```

                   mean     sum    max
    Department                        
    Finance     65000.0   65000  65000
    HR          47500.0   95000  50000
    IT          65000.0  130000  70000



```python

```


```python
#Merging, Joining, and Concatenating
```


```python
df1 = pd.DataFrame({'ID': [1, 2], 'Name': ['Alice', 'Bob']})
df2 = pd.DataFrame({'ID': [1, 3], 'Salary': [50000, 60000]})
```


```python
merged = pd.merge(df1, df2, on='ID', how='outer')
print(merged)
```

       ID   Name   Salary
    0   1  Alice  50000.0
    1   2    Bob      NaN
    2   3    NaN  60000.0



```python

```


```python
#Concatenating
```


```python
concat = pd.concat([df1, df2], ignore_index=True)
print(concat)
```

       ID   Name   Salary
    0   1  Alice      NaN
    1   2    Bob      NaN
    2   1    NaN  50000.0
    3   3    NaN  60000.0



```python

```


```python

```


```python

```


---
**Score: 15**
