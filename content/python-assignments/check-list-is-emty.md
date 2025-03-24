---
title: Check-List-Is-Emty
date: 2025-03-24
author: Your Name
cell_count: 5
score: 5
---

```python
#Write a function to check if a list is empty.
```


```python
def is_list_empty(lst):
    """
    Check if a list is empty.

    Parameters:
    lst (list): A list to check for emptiness.

    Returns:
    bool: True if the list is empty, False otherwise.
    """

    # Check if the list is empty
    if lst == []:
        return True
        
    return False
```


```python
# Sample test cases
print(is_list_empty([])) # True
```

    True



```python
print(is_list_empty([1, 2, 3])) # False
```

    False



```python

```


---
**Score: 5**
