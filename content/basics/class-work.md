---
title: Class-Work
date: 2024-11-19
author: Your Name
cell_count: 5
score: 5
---

```python
class Person:  
    """
    revisit the Person class to validate argument
    """
    def __init__(self, name, job, pay):
        self.job  = job
        self.pay  = pay
                                          # arg 0 is the self instance here
                                          # giveRaise = rangetest(..)(giveRaise)
    def giveRaise(self, percent):
        self.pay = int(self.pay * (1 + percent))
```


```python
sue = Person('Sue Jones', 'dev', 100000)
```


```python
sue
```




    <__main__.Person at 0x7fcaddf177d0>




```python
sue.pay
```




    100000




```python

```


---
**Score: 5**