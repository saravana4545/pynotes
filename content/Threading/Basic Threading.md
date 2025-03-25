---
title: Basic Threading
date: 2025-03-25
author: Your Name
cell_count: 6
score: 5
---

```python
# created 25-03-2025
```


```python
# Threading & Multiprocessing
```


```python
import threading
```


```python
def print_numbers():
    for i in range(5):
        print(i)
```


```python
t = threading.Thread(target=print_numbers)
t.start()
t.join()
```

    0
    1
    2
    3
    4



```python

```


---
**Score: 5**
