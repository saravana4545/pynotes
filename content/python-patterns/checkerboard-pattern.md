---
title: Checkerboard-Pattern
date: 2025-01-02
author: Your Name
cell_count: 4
score: 0
---

```python
# checkerboard pattern
```


```python
def checkerboard():
    rows = 5
    for i in range(1, rows + 1):
        for j in range(1, rows + 1):
            if (i + j) % 2 == 0:
                print("1", end=" ")
            else:
                print("0", end=" ")
        print()
```


```python
checkerboard()
```

    1 0 1 0 1 
    0 1 0 1 0 
    1 0 1 0 1 
    0 1 0 1 0 
    1 0 1 0 1 



```python

```


---
**Score: 0**
