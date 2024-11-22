---
title: Numpy-Lib
date: 2024-11-22
author: Your Name
cell_count: 6
score: 5
---

```python
import numpy as np;
```


```python
import random
```


```python
np.random.seed(123);
```


```python
def coin_twist():
    for num in range(1,20):
        coin = np.random.randint(0, 3);
        print(coin);
        if(coin == 0):
            return "heads"
        else:
            return "tails"
```


```python
print(coin_twist())
```

    1
    tails



```python

```


---
**Score: 5**
