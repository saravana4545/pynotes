---
title: Filtering-And-Querying-Pd
date: 2024-12-08
author: Your Name
cell_count: 22
score: 20
---

```python

```


```python
import pandas as pd
```


```python
#Filtering and Querying
```


```python
data = {
    'Name': ['Alice', 'Bob', 'Charlie'],
    'Age': [25, 30, 35],
    'Salary': [50000, 60000, 70000]
}
```


```python
df = pd.DataFrame(data)
```


```python
# Querying the DataFrame
```


```python
filtered = df.query('Age > 28 and Salary > 55000')
print(filtered)
```

          Name  Age  Salary
    1      Bob   30   60000
    2  Charlie   35   70000



```python

```


```python

```


```python
#Filtering with Complex Conditions
```


```python
# Using lambda functions
```


```python
filtered = df[df['Name'].apply(lambda x: x.startswith('A'))]
print(filtered)
```

        Name  Age  Salary
    0  Alice   25   50000



```python

```


```python
#Data Transformation and Adding Calculated Columns
```


```python
df['Salary in USD'] = df['Salary'] * 1.1  # Assuming a 10% conversion rate
print(df)
```

          Name  Age  Salary  Salary in USD
    0    Alice   25   50000        55000.0
    1      Bob   30   60000        66000.0
    2  Charlie   35   70000        77000.0



```python

```


```python

```


```python
#Apply Custom Functions
```


```python
def age_group(age):
    if age < 30:
        return 'Young'
    elif age < 40:
        return 'Mid-Age'
    else:
        return 'Senior'
```


```python
df['Age Group'] = df['Age'].apply(age_group)
print(df)
```

          Name  Age  Salary  Salary in USD Age Group
    0    Alice   25   50000        55000.0     Young
    1      Bob   30   60000        66000.0   Mid-Age
    2  Charlie   35   70000        77000.0   Mid-Age



```python

```


```python

```


---
**Score: 20**
