---
title: Arthmetic-Error
date: 2024-12-23
author: Your Name
cell_count: 4
score: 0
---

```python
# ArithmeticError
```


```python
def my_function(x,y):
    try:
        result = x ** y
        return result
    except OverflowError as e:
        print(f"OverflowError occurred: {e}")
```


```python
print(my_function(100,100))
```

    100000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000



```python

```


---
**Score: 0**
