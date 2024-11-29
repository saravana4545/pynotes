---
title: Assign7-Calculate
date: 2024-11-29
author: Your Name
cell_count: 4
score: 0
---

```python
#Calculates the sum of its digits.Prints the result.
```


```python
def sum_of_digits(num):
    digit_sum = 0
    while num > 0:
        digit_sum += num % 10
        num //= 10
    return digit_sum
```


```python
list = 4545
print(sum_of_digits(list)) 
```

    18



```python

```


---
**Score: 0**
