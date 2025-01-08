---
title: Logging-Lib
date: 2025-01-08
author: Your Name
cell_count: 7
score: 5
---

```python
#import neccessery libraries
```


```python
import logging
```


```python
#This Configures logging level, format, and output details for messages.
```


```python
logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(levelname)s - %(message)s')
```


```python
#It's doing lots of alert messages
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
**Score: 5**
