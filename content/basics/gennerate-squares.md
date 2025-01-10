---
title: Gennerate-Squares
date: 2025-01-10
author: Your Name
cell_count: 5
score: 5
---

```python
def generate_squares(n):
    """
    Generate a list of squares of numbers from 1 to n.

    Parameters:
    n (int): The upper limit of the range.

    Returns:
    list: A list of squares of numbers from 1 to n.
    """
    
    squares = [n ** 2 for n in range(1, n+1)]
    return squares
```


```python
# Sample test cases
```


```python
print(generate_squares(5))# Expected output: [1, 4, 9,16,25]
```

    [1, 4, 9, 16, 25]



```python
print(generate_squares(3))
```

    [1, 4, 9]



```python

```


---
**Score: 5**
