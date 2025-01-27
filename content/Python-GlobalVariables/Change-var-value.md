---
title: Change-Var-Value
date: 2025-01-27
author: Your Name
cell_count: 7
score: 5
---

```python
# Created at 20-01-2025
```


```python
# https://www.scientecheasy.com/2022/09/global-and-local-variables-in-python.html/
```


```python
# we need to write a global keyword before the variable name inside the function.
```


```python
name = "andal"
```


```python
def change_value():
    global name
    name = "andal priya"
    print("Full name is", name)
```


```python
change_value()
print("The Modified name is", name)
```

    Full name is andal priya
    The Modified name is andal priya



```python

```


---
**Score: 5**
