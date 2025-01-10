---
title: Groupby-And-Aggregation
date: 2025-01-10
author: Your Name
cell_count: 17
score: 15
---

```python
#GroupBy with Multiple Aggregations
```


```python
#import pandas library
```


```python
import pandas as pd
```


```python
# Sample DataFrame
```


```python

```


```python
data = {
    'Department': ['HR', 'HR', 'IT', 'IT', 'Sales', 'Sales'],
    'Employee': ['John', 'Emma', 'Alice', 'Bob', 'Charles', 'Diana'],
    'Salary': [50000, 60000, 75000, 80000, 45000, 48000],
    'Experience': [5, 4, 6, 7, 3, 2]
}

```


```python
#convert the variable as DataFrame
```


```python
df = pd.DataFrame(data)
```


```python
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Department</th>
      <th>Employee</th>
      <th>Salary</th>
      <th>Experience</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>HR</td>
      <td>John</td>
      <td>50000</td>
      <td>5</td>
    </tr>
    <tr>
      <th>1</th>
      <td>HR</td>
      <td>Emma</td>
      <td>60000</td>
      <td>4</td>
    </tr>
    <tr>
      <th>2</th>
      <td>IT</td>
      <td>Alice</td>
      <td>75000</td>
      <td>6</td>
    </tr>
    <tr>
      <th>3</th>
      <td>IT</td>
      <td>Bob</td>
      <td>80000</td>
      <td>7</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Sales</td>
      <td>Charles</td>
      <td>45000</td>
      <td>3</td>
    </tr>
    <tr>
      <th>5</th>
      <td>Sales</td>
      <td>Diana</td>
      <td>48000</td>
      <td>2</td>
    </tr>
  </tbody>
</table>
</div>




```python
# Group by and aggregate
```


```python

```


```python
agg_df = df.groupby('Department').agg(
    Total_Salary=('Salary', 'sum'),
    Avg_Experience=('Experience', 'mean'),
    Max_Salary=('Salary', 'max')
).reset_index()
```


```python
print(f"Grouped and Aggregated DataFrame:\n{agg_df}")
```

    Grouped and Aggregated DataFrame:
      Department  Total_Salary  Avg_Experience  Max_Salary
    0         HR        110000             4.5       60000
    1         IT        155000             6.5       80000
    2      Sales         93000             2.5       48000



```python

```


```python

```


```python

```


```python

```


---
**Score: 15**
