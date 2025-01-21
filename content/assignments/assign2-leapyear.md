---
title: Assign2-Leapyear
date: 2025-01-21
author: Your Name
cell_count: 6
score: 5
---

```python
#Find its leap year or not
```


```python
#create method called leap_year
```


```python
def leap_year(year):
    if (year % 4 == 0 and year % 100 != 0):
        return f"{year} is a leap year."
    else:
        return f"{year} is not a leap year."
```


```python
#put a range for it and print
```


```python
for i in range (1996,2000):
    print(leap_year(i))
```

    1996 is a leap year.
    1997 is not a leap year.
    1998 is not a leap year.
    1999 is not a leap year.



```python

```


---
**Score: 5**
