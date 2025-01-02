---
title: Check-Palindrome
date: 2025-01-02
author: Your Name
cell_count: 6
score: 5
---

```python
#Write a function to check if a string is a palindrome.
```


```python
def is_palindrome(s):
    """
    Problem: Write a function to check if a string is a palindrome.
    
    Args:
    s: input string to be checked
    
    Returns:
    True if the string is a palindrome, False otherwise
    """
    if s == s[::-1]:
        return True
    return False
```


```python
# Sample test cases
print(is_palindrome("racecar"))  # True
```

    True



```python
print(is_palindrome("hello"))    # False
```

    False



```python
print(is_palindrome("level"))    # True
```

    True



```python

```


---
**Score: 5**
