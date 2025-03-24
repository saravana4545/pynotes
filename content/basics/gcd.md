---
title: Gcd
date: 2025-03-24
author: Your Name
cell_count: 5
score: 5
---

```python
#create a method called gcd()
```


```python
def gcd(a, b):
    if b == 0:  
        return a
    else:
        return gcd(b, a % b)
```


```python
#put the values for a and b by calling the method
```


```python
print(gcd(17, 23))
```

    1



```python

```


---
**Score: 5**
