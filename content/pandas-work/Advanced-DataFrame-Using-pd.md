---
title: Advanced-Dataframe-Using-Pd
date: 2025-01-08
author: Your Name
cell_count: 26
score: 25
---

```python
#import pandas library
```


```python
#!pip install pandas
```


```python
import pandas as pd
```


```python
#create a variable called data and put some values
```


```python
data1 = {
    'Category': ['A', 'A', 'B', 'B'],
    'Type': ['X', 'Y', 'X', 'Y'],
    'Value': [10, 20, 30, 40]
}
```


```python
df = pd.DataFrame(data1)
```


```python
# Setting a multi-level index
```


```python
df = df.set_index(['Category', 'Type'])
print(df)
```

                   Value
    Category Type       
    A        X        10
             Y        20
    B        X        30
             Y        40



```python
# Accessing data using multi-level indexing
```


```python
print(df.loc['A', 'X'])
```

    Value    10
    Name: (A, X), dtype: int64



```python

```


```python

```


```python
#create pivot  table 
```


```python
data2 = {
    'City': ['New York', 'Los Angeles', 'Chicago', 'New York'],
    'Year': [2020, 2020, 2021, 2021],
    'Sales': [100, 200, 150, 300]
}
```


```python
df = pd.DataFrame(data2)
```


```python
# Creating a pivot table
```


```python
pivot = df.pivot_table(values='Sales', index='City', columns='Year', aggfunc='sum', fill_value=0)
print(pivot)
```

    Year         2020  2021
    City                   
    Chicago         0   150
    Los Angeles   200     0
    New York      100   300



```python

```


```python

```


```python
#Exploding Lists into Rows
```


```python
data3 = {
    'Name': ['Alice', 'Bob'],
    'Hobbies': [['Reading', 'Cycling'], ['Swimming']]
}
```


```python
df = pd.DataFrame(data3)
```


```python
# Exploding lists into separate rows
```


```python
df = df.explode('Hobbies')
print(df)
```

        Name   Hobbies
    0  Alice   Reading
    0  Alice   Cycling
    1    Bob  Swimming



```python

```


```python

```


---
**Score: 25**
