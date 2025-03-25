---
title: Log Decorator
date: 2025-03-25
author: Your Name
cell_count: 5
score: 5
---

```python
# Created at 24-03-2025
```


```python
# Logging Decorator
```


```python
def log_function_call(func):
    def wrapper(*args, **kwargs):
        print(f"Calling {func.__name__} with arguments {args} {kwargs}")
        return func(*args, **kwargs)
    return wrapper
```


```python
@log_function_call
def add(a, b, num):
    return a + b + num

print(add(5, 3,num=4))
```

    Calling add with arguments (5, 3) {'num': 4}
    12



```python

```


---
**Score: 5**
