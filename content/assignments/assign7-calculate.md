---
title: Assign7-Calculate
date: 2024-12-23
author: Your Name
cell_count: 6
score: 5
---

```python
#Calculates the sum of its digits.Prints the result.
```


```python
#create method called sum_of_digits()
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
#create a variable and put the value for num
```


```python
list = 4545
print(sum_of_digits(list)) 
```

    18



```python

```


---
**Score: 5**
