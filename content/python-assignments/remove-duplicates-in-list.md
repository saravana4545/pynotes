---
title: Remove-Duplicates-In-List
date: 2025-01-30
author: Your Name
cell_count: 6
score: 5
---

```python
#9. Write a function to remove duplicates from a list.
```


```python
def remove_duplicates(lst):
    """
    Problem: Write a function to remove duplicates from a list.
    
    Args:
    lst: a list of elements
    
    Returns:
    a list with duplicates removed
    """
    remove_duplicate = list(dict.fromkeys(lst))
    
    return remove_duplicate
```


```python
# Sample test cases
```


```python
print(remove_duplicates([1, 2, 2, 3, 4, 4, 5])) # Output: [1, 2, 3, 4, 5]
```

    [1, 2, 3, 4, 5]



```python
print(remove_duplicates(['a', 'b', 'a', 'c', 'd', 'b'])) # Output: ['a', 'b', 'c', 'd']
```

    ['a', 'b', 'c', 'd']



```python

```


---
**Score: 5**
