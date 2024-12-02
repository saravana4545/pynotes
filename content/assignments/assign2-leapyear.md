---
title: Assign2-Leapyear
date: 2024-12-02
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
for i in range (2020,2025):
    print(leap_year(i))
```

    2020 is a leap year.
    2021 is not a leap year.
    2022 is not a leap year.
    2023 is not a leap year.
    2024 is a leap year.



```python

```


---
**Score: 5**
