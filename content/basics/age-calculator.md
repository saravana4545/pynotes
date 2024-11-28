---
title: Age-Calculator
date: 2024-11-28
author: Your Name
cell_count: 5
score: 5
---

```python
from datetime import datetime
```


```python
def get_age(d):
    d1 = datetime.now()
    months = (d1.year - d.year) * 12 + d1.month - d.month

    year = int(months / 12)
    return year
```


```python
age = get_age(datetime(2003))
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    Cell In[6], line 1
    ----> 1 age = get_age(datetime(2003))


    NameError: name 'get_age' is not defined



```python
age
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    Cell In[5], line 1
    ----> 1 age


    NameError: name 'age' is not defined



```python

```


---
**Score: 5**
