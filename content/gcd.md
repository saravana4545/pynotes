---
title: Gcd
date: 2024-11-29
author: Your Name
cell_count: 3
score: 0
---

```python
def gcd(a, b):
    if b == 0:  
        return a
    else:
        return gcd(b, a % b)
    
```


```python
print(gcd(17, 23))
```

    1



```python

```


---
**Score: 0**
