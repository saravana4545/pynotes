---
title: Numpy-Lib
date: 2024-11-23
author: Your Name
cell_count: 5
score: 5
---

```python
import numpy as np;
```


```python
import random
```


```python
def coin_twist():
    for num in range(1,20):
        coin = random.randint(0, 3);
        print(coin);
        if(coin == 0):
            return "heads"
        else:
            return "tails"
```


```python
print(coin_twist())
```

    3
    tails



```python

```


---
**Score: 5**
