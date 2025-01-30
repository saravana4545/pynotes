---
title: Sorted-List
date: 2025-01-30
author: Your Name
cell_count: 6
score: 5
---

```python
#8. Write a function to sort a list in ascending order.
```


```python
def sort_list_ascending(lst):
    """
    Sort a list in ascending order.

    Parameters:
    lst (list): List to be sorted.

    Returns:
    list: Sorted list in ascending order.
    """
    sorted_list = sorted(lst)

    return sorted_list
```


```python
# Sample test cases
```


```python
print(sort_list_ascending([3, 1, 4, 1, 5, 9, 2, 6, 5, 3]))  # Expected output: [1, 1, 2, 3, 3, 4, 5, 5, 6, 9]
```

    [1, 1, 2, 3, 3, 4, 5, 5, 6, 9]



```python
print(sort_list_ascending([9, 8, 7, 6, 5, 4, 3, 2, 1]))  # Expected output: [1, 2, 3, 4, 5, 6, 7, 8, 9]
```

    [1, 2, 3, 4, 5, 6, 7, 8, 9]



```python

```


---
**Score: 5**
