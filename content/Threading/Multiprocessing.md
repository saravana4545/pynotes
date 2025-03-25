---
title: Multiprocessing
date: 2025-03-25
author: Your Name
cell_count: 5
score: 5
---

```python
# Created at 25-03-2025
```


```python
# Using multiprocessing to Run Functions in Parallel
```


```python
import multiprocessing
import time
```


```python
def worker(n):
    print(f"Worker {n} started")
    time.sleep(2)
    print(f"Worker {n} finished")
```


```python
if __name__ == "__main__":
    processes = []
    for i in range(4):
        p = multiprocessing.Process(target=worker, args=(i,))
        processes.append(p)
        p.start()
    for p in processes:
        p.join()

    print("All workers completed.")
```

    Worker 1 started
    Worker 2 started
    Worker 3 started
    Worker 0 started
    Worker 1 finished
    Worker 2 finished
    Worker 3 finished
    Worker 0 finished
    All workers completed.



---
**Score: 5**
