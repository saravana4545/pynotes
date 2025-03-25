---
title: Check-Is-Leap-Year
date: 2025-03-25
author: Your Name
cell_count: 9
score: 5
---

```python
#Write a function to check if a given year is a leap year.
```


```python
def is_leap_year(year):
    """
    Given a year, check if it is a leap year.

    Parameters:
    year (int): The year to be checked.

    Returns:
    bool: True if the year is a leap year, False otherwise.
    """

    # Check if the year is divisible by 4
    if (year % 4==0 and year % 100 != 0):
        return True
    else:
        return False
```


```python
# Sample test cases
print(is_leap_year(2000)) # Expected output: True
```

    False



```python
print(is_leap_year(1900)) # Expected output: False
```

    False



```python
print(is_leap_year(2021)) # Expected output: False
```

    False



```python
print(is_leap_year(2002)) 
```

    False



```python
print(is_leap_year(1996))
```

    True



```python

```


```python

```


---
**Score: 5**
