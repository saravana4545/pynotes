---
title: Find-Prime-Num
date: 2025-01-21
author: Your Name
cell_count: 7
score: 5
---

```python
#7. Write a function to check if a number is prime.
```


```python
def is_prime(num):
    """
    Check if a number is prime.

    Parameters:
    num (int): The number to check for primality.

    Returns:
    bool: True if the number is prime, False otherwise.
    """
    if num % 2:
        return True

    return False
```


```python
# Sample test cases
```


```python
print(is_prime(5)) # Expected output: True
```

    True



```python
print(is_prime(10)) # Expected output: False
```

    False



```python
print(is_prime(17)) # Expected output: True
```

    True



```python

```


---
**Score: 5**
