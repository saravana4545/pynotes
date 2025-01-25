---
title: Alphabet Pattern
date: 2025-01-25
author: Your Name
cell_count: 3
score: 0
---

```python
def alphabet_pattern():
    rows = 5
    for i in range(1, rows + 1):
        print(" " * (rows - i) + " ".join(chr(65 + j) for j in range(i)))
```


```python
alphabet_pattern()
```

        A
       A B
      A B C
     A B C D
    A B C D E



```python

```


---
**Score: 0**
