---
title: Pivot-Table-Using-Pandas
date: 2024-12-08
author: Your Name
cell_count: 17
score: 15
---

```python
#Pivot Tables for Aggregated Data Analysis
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
    'Category': ['A', 'A', 'B', 'B', 'C', 'C'],
    'Subcategory': ['X', 'Y', 'X', 'Y', 'X', 'Y'],
    'Values': [10, 20, 0, 40, 50, 60],
    'Counts': [1, 2, 1, 3, 2, 4]
}
```


```python
#converte the variable as DataFrame
```


```python

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
      <th>Category</th>
      <th>Subcategory</th>
      <th>Values</th>
      <th>Counts</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>A</td>
      <td>X</td>
      <td>10</td>
      <td>1</td>
    </tr>
    <tr>
      <th>1</th>
      <td>A</td>
      <td>Y</td>
      <td>20</td>
      <td>2</td>
    </tr>
    <tr>
      <th>2</th>
      <td>B</td>
      <td>X</td>
      <td>0</td>
      <td>1</td>
    </tr>
    <tr>
      <th>3</th>
      <td>B</td>
      <td>Y</td>
      <td>40</td>
      <td>3</td>
    </tr>
    <tr>
      <th>4</th>
      <td>C</td>
      <td>X</td>
      <td>50</td>
      <td>2</td>
    </tr>
    <tr>
      <th>5</th>
      <td>C</td>
      <td>Y</td>
      <td>60</td>
      <td>4</td>
    </tr>
  </tbody>
</table>
</div>




```python
# Create a pivot table
```


```python

```


```python
pivot = pd.pivot_table(
    df, 
    values='Values', 
    index='Category', 
    columns='Subcategory', 
    aggfunc='sum', 
    fill_value=0
)
```


```python
print("Pivot Table:")
print(pivot)
```

    Pivot Table:
    Subcategory   X   Y
    Category           
    A            10  20
    B             0  40
    C            50  60



```python

```


```python

```


```python

```


---
**Score: 15**
