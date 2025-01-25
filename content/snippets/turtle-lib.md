---
title: Turtle-Lib
date: 2025-01-25
author: Your Name
cell_count: 7
score: 5
---

```python
#import neccessery libraries
```


```python
import turtle
```


```python
#create a method called home()
```


```python
def home():
    screen = turtle.Screen()
    t      = turtle.Turtle()
    for _ in range(4):
        t.forward(100)
        t.right(90)
    turtle.done()
    return turtle
```


```python
#call the method using print
```


```python
print(home())
```

    <module 'turtle' from '/home/saravanakumar/miniconda3/envs/py12/lib/python3.12/turtle.py'>



```python

```


---
**Score: 5**
