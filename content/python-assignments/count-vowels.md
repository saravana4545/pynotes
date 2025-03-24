---
title: Count-Vowels
date: 2025-03-24
author: Your Name
cell_count: 7
score: 5
---

```python
#6. Write a function to count the vowels in a string.
```


```python
def count_vowels(s):
    """
    This function counts the number of vowels in a given string.
    
    Parameters:
    s (str): A string to count vowels from.
    
    Returns:
    int: The number of vowels in the string.
    """
    
    # Initialize a variable to store the count of vowels
    vowels = ('a','e','i','o','u')
    count  = 0
    # Loop through each character in the string
    for items in vowels:
        count += s.count(items)
    return count
```


```python
# Test cases
```


```python
print(count_vowels("hello")) # Expected output: 2
```

    2



```python
print(count_vowels("Python")) # Expected output: 1
```

    1



```python
print(count_vowels("programming")) # Expected output: 3
```

    3



```python

```


---
**Score: 5**
