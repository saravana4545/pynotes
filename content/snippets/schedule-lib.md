---
title: Schedule-Lib
date: 2025-03-25
author: Your Name
cell_count: 6
score: 5
---

```python
import schedule
```


```python
import time
```


```python
def job():
    print("This task runs every 5 seconds.")
```


```python
schedule.every(5).seconds.do(job)

while True:
    schedule.run_pending()
    time.sleep(1)
```


```python

```


```python

```


---
**Score: 5**
