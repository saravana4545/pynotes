---
title: Not
date: 2025-01-30
author: Your Name
cell_count: 6
score: 5
---

```python
# Created at 21-01-2025
```


```python
# https://www.scientecheasy.com/2022/10/identity-operators-in-python.html/
```


```python
# Identity Is not operator (is not).
```


```python
def not_operator():
    num1 = id(10)
    num2 = id(10)
    result = (num1, num2)
    if num1 is not num2:
        print("num1 & num2 have the same id-",result)
    else:
        print("num1 & num2 is not same id.", result)
```


```python
not_operator()
```

    num1 & num2 have the same id- (9767048, 9767048)



```python

```


---
**Score: 5**
