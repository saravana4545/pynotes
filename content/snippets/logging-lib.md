---
title: Logging-Lib
date: 2024-11-23
author: Your Name
cell_count: 4
score: 0
---

```python
import logging
```


```python
logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(levelname)s - %(message)s')
```


```python
logging.debug("This is a debug message")
logging.info("This is an info message")
logging.warning("This is a warning message")
logging.error("This is an error message")
logging.critical("This is a critical message")
```

    2024-11-23 07:35:25,460 - DEBUG - This is a debug message
    2024-11-23 07:35:25,462 - INFO - This is an info message
    2024-11-23 07:35:25,464 - WARNING - This is a warning message
    2024-11-23 07:35:25,465 - ERROR - This is an error message
    2024-11-23 07:35:25,466 - CRITICAL - This is a critical message



```python

```


---
**Score: 0**
