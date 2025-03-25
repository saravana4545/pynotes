---
title: Sum-Of-Numbers
date: 2025-03-25
author: Your Name
cell_count: 6
score: 5
---

```python
#5. Write a function to calculate the sum of numbers in a list.
```


```python
def calculate_sum(numbers):
    """
    Calculate the sum of numbers in a list.

    Parameters:
    numbers (list): A list of numbers to calculate the sum for.

    Returns:
    int: The sum of numbers in the list.
    """
    add_list = sum(numbers)
    return add_list
```


```python
#Sample test cases
```


```python
print(calculate_sum([1, 2, 3])) # Expected output: 6
```

    6



```python
print(calculate_sum([-1, 0, 1])) # Expected output: 0
```

    0



```python

```


---
**Score: 5**
