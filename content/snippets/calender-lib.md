---
title: Calender-Lib
date: 2024-12-21
author: Your Name
cell_count: 8
score: 5
---

```python
#import the calendor library
```


```python
import calendar
```


```python
#create a variable and put some random year
```


```python
year = 2023
print(f"Is {year} a leap year?", calendar.isleap(year))
```

    Is 2023 a leap year? False



```python
#print the variable
```


```python
print("\nMonthly Calendar:")
print(calendar.month(year, 11))
```

    
    Monthly Calendar:
       November 2024
    Mo Tu We Th Fr Sa Su
                 1  2  3
     4  5  6  7  8  9 10
    11 12 13 14 15 16 17
    18 19 20 21 22 23 24
    25 26 27 28 29 30
    



```python
print("\nYear Calendar:")
print(calendar.TextCalendar().formatyear(2025))
```

    
    Year Calendar:
                                      2025
    
          January                   February                   March
    Mo Tu We Th Fr Sa Su      Mo Tu We Th Fr Sa Su      Mo Tu We Th Fr Sa Su
           1  2  3  4  5                      1  2                      1  2
     6  7  8  9 10 11 12       3  4  5  6  7  8  9       3  4  5  6  7  8  9
    13 14 15 16 17 18 19      10 11 12 13 14 15 16      10 11 12 13 14 15 16
    20 21 22 23 24 25 26      17 18 19 20 21 22 23      17 18 19 20 21 22 23
    27 28 29 30 31            24 25 26 27 28            24 25 26 27 28 29 30
                                                        31
    
           April                      May                       June
    Mo Tu We Th Fr Sa Su      Mo Tu We Th Fr Sa Su      Mo Tu We Th Fr Sa Su
        1  2  3  4  5  6                1  2  3  4                         1
     7  8  9 10 11 12 13       5  6  7  8  9 10 11       2  3  4  5  6  7  8
    14 15 16 17 18 19 20      12 13 14 15 16 17 18       9 10 11 12 13 14 15
    21 22 23 24 25 26 27      19 20 21 22 23 24 25      16 17 18 19 20 21 22
    28 29 30                  26 27 28 29 30 31         23 24 25 26 27 28 29
                                                        30
    
            July                     August                  September
    Mo Tu We Th Fr Sa Su      Mo Tu We Th Fr Sa Su      Mo Tu We Th Fr Sa Su
        1  2  3  4  5  6                   1  2  3       1  2  3  4  5  6  7
     7  8  9 10 11 12 13       4  5  6  7  8  9 10       8  9 10 11 12 13 14
    14 15 16 17 18 19 20      11 12 13 14 15 16 17      15 16 17 18 19 20 21
    21 22 23 24 25 26 27      18 19 20 21 22 23 24      22 23 24 25 26 27 28
    28 29 30 31               25 26 27 28 29 30 31      29 30
    
          October                   November                  December
    Mo Tu We Th Fr Sa Su      Mo Tu We Th Fr Sa Su      Mo Tu We Th Fr Sa Su
           1  2  3  4  5                      1  2       1  2  3  4  5  6  7
     6  7  8  9 10 11 12       3  4  5  6  7  8  9       8  9 10 11 12 13 14
    13 14 15 16 17 18 19      10 11 12 13 14 15 16      15 16 17 18 19 20 21
    20 21 22 23 24 25 26      17 18 19 20 21 22 23      22 23 24 25 26 27 28
    27 28 29 30 31            24 25 26 27 28 29 30      29 30 31
    



```python

```


---
**Score: 5**
