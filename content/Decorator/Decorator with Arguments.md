---
title: Decorator With Arguments
date: 2025-03-25
author: Your Name
cell_count: 6
score: 5
---

```python
# Created at 24-03-2025
```


```python
# Decorator with Arguments
```


```python
# Why Use *args and **kwargs?

    # The decorator should work with any function, regardless of how many arguments it takes.

    # Without *args, **kwargs, the decorator would only work for functions with a fixed number of arguments.
```


```python
def repeat(n):
    def decorator(func):
        def wrapper(*args, **kwargs):
            for _ in range(n):
                func(*args, **kwargs)
        return wrapper
    return decorator
```


```python
@repeat(3)
def greet():
    print("Hi!")

greet()
```

    Hi!
    Hi!
    Hi!



```python

```


---
**Score: 5**
