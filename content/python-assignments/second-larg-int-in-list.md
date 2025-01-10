---
title: Second-Larg-Int-In-List
date: 2025-01-10
author: Your Name
cell_count: 7
score: 5
---

```python
# https://stackoverflow.com/questions/16225677/get-the-second-largest-number-in-a-list-in-linear-time
```


```python
#15 - Write a function to find the second largest number in a list.
```


```python
def find_second_largest(arr):
    """
    Given a list of integers, find the second largest number in the list.

    Parameters:
    arr (list): A list of integers

    Returns:
    int: The second largest number in the list
    """
    
    # Sort the list in descending order
    sort_list = sorted(arr)[-2]
    return sort_list
```


```python
# Sample test cases
```


```python
print(find_second_largest([1, 2, 3, 4, 5])) # Expected output: 4
```

    4



```python
print(find_second_largest([10, 5, 20, 15, 30])) # Expected output: 20
```

    20



```python

```


---
**Score: 5**
