---
title: Find-Index
date: 2025-03-24
author: Your Name
cell_count: 6
score: 5
---

```python
def find_index(item, lst):
    """
    This function finds the index of an item in a list.

    Parameters:
    item (any): The item to find in the list.
    lst (list): The list to search for the item.

    Returns:
    int: The index of the item in the list, or -1 if the item is not found.
    """
    try:
        list_index = lst.index(item)
        return list_index
    except:
        return "-1"
```


```python
# Sample test cases
```


```python
print(find_index(3, [1, 2, 3, 4, 5]))  # Expected output: 2
```

    2



```python
print(find_index('a', ['a', 'b', 'c']))  # Expected output: 0
```

    0



```python
print(find_index(6, [1, 2, 3, 4, 5]))  # Expected output: -1
```

    -1



```python

```


---
**Score: 5**
