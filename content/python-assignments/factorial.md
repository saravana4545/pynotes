---
title: Factorial
date: 2025-03-27
author: Your Name
cell_count: 7
score: 5
---

```python
#https://stackoverflow.com/questions/76722924/calculate-the-factorial-of-a-number
```


```python
#Write a function to calculate the factorial of a number.
```


```python
def factorial(n):
    """
    Calculate the factorial of a number.

    Parameters:
    n (int): The number to calculate the factorial for.

    Returns:
    int: The factorial of the given number.
    """
    if n == 0:
        return 1
    else:
        return n*factorial(n-1)
```


```python
# Sample test cases
print(factorial(0)) # Expected output: 1
```

    1



```python
print(factorial(5)) # Expected output: 120
```

    120



```python
print(factorial(10)) # Expected output: 3628800
```

    3628800



```python

```


---
**Score: 5**
