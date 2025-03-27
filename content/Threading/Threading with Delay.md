---
title: Threading With Delay
date: 2025-03-27
author: Your Name
cell_count: 4
score: 0
---

```python
# Created at 25-03-2025
```


```python
# Threading with Delay
```


```python
import threading
import time

def delayed_print(msg):
    time.sleep(2)
    print(msg)

t = threading.Thread(target=delayed_print, args=("Hello, after delay!",))
t.start()
```

    Hello, after delay!



```python

```


---
**Score: 0**
