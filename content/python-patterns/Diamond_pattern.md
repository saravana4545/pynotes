---
title: Diamond Pattern
date: 2025-01-21
author: Your Name
cell_count: 4
score: 0
---

```python
# create diaamond pattern
```


```python
def diamond_shape():
    rows = 5
    for i in range(1, rows + 1):
        print(" " * (rows - i) + "* " * i)
    for i in range(rows - 1, 0, -1):
        print(" " * (rows - i) + "* " * i)
```


```python
diamond_shape()
```

        * 
       * * 
      * * * 
     * * * * 
    * * * * * 
     * * * * 
      * * * 
       * * 
        * 



```python

```


---
**Score: 0**
