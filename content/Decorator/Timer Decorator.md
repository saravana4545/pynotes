---
title: Timer Decorator
date: 2025-03-27
author: Your Name
cell_count: 7
score: 5
---

```python
# Created at 24-03-2025
```


```python
# Timer Decorator
```


```python
import time
```


```python
def timer(func):
    def wrapper(*args, **kwargs):
        start = time.time()
        result = func(*args, **kwargs)
        end = time.time()
        print(f"Execution time: {end - start:.4f} seconds") # .4f - It prints with four decimal places.
        return result
    return wrapper
```


```python
@timer
def slow_function():
    time.sleep(1)
    print("Done")
```


```python
slow_function()
```

    Done
    Execution time: 1.0002 seconds



```python

```


---
**Score: 5**
