---
title: Check-Num-Positive-Ornot
date: 2025-01-20
author: Your Name
cell_count: 7
score: 5
---

```python
# 23 - Write a function to check if a number is positive, negative, or zero.
```


```python
def check_number(num):
    """
    This function checks if a number is positive, negative, or zero.

    Parameters:
    num (int): The number to be checked.

    Returns:
    str: 'Positive' if the number is positive, 'Negative' if the number is negative, 'Zero' if the number is zero.
    """
    if num == 0:
        return "Zero"
    elif num >= 0:
        return "positive"

    return "negative"
```


```python
# Sample test cases
```


```python
print(check_number(5))  # Expected output: 'Positive'
```

    positive



```python
print(check_number(-3))  # Expected output: 'Negative'
```

    negative



```python
print(check_number(0))  # Expected output: 'Zero'
```

    Zero



```python

```


---
**Score: 5**
