---
title: Occurrences-Count
date: 2025-01-08
author: Your Name
cell_count: 6
score: 5
---

```python
#Write a function to count the occurrences of an item in a list.
```


```python
def count_occurrences(lst, item):
    """
    Count the occurrences of an item in a list.

    Parameters:
    lst (list): The list to search for occurrences.
    item: The item to count occurrences of.

    Returns:
    int: The number of occurrences of the item in the list.
    """
    
    # TODO: Implement the function
    count_occur = lst.count(item)
    return count_occur
```


```python
# Sample test cases
```


```python
print(count_occurrences([1, 2, 2, 3, 4, 2], 2))  # Output: 3
```

    3



```python
print(count_occurrences(['a', 'b', 'c', 'a', 'a'], 'a'))  # Output: 3
```

    3



```python

```


---
**Score: 5**
