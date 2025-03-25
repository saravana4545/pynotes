---
title: Basic Decorator
date: 2025-03-25
author: Your Name
cell_count: 5
score: 5
---

```python
# Created at 24-03-2025
```


```python
# Basic Decorator
```


```python
def decorator(func):
    def wrapper():
        print("Before function call")
        func()
        print("After function call")
    return wrapper
```


```python
@decorator
def say_hello():
    print("Hello, World!")

say_hello()
```

    Before function call
    Hello, World!
    After function call



```python

```


---
**Score: 5**
