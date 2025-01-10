---
title:  Time-Series-Analysis
date: 2025-01-10
author: Your Name
cell_count: 12
score: 10
---

```python
#import neccessary library
```


```python
import pandas as pd
```


```python
# Creating a DataFrame with time series data
```


```python
time_data = {
    'Date': pd.date_range(start='2023-01-01', periods=5),
    'Value': [10, 20, 30, 40, 50]
}
```


```python
df = pd.DataFrame(time_data)
```


```python
# Setting the Date column as the index
```


```python
df = df.set_index('Date')
```


```python
# Resampling to a different frequency (weekly)
```


```python
resampled = df.resample('W').sum()
print(resampled)
```

                Value
    Date             
    2023-01-01     10
    2023-01-08    140



```python

```


```python

```


```python

```


---
**Score: 10**
