---
title: Datatime-Using-Pytz-Lib
date: 2024-11-26
author: Your Name
cell_count: 6
score: 5
---

```python
from datetime import datetime
```


```python
import pytz
```


```python
utc   = pytz.utc
local = pytz.timezone('Asia/kolkata')
```


```python
utc_time   = datetime.now(utc)
local_time = utc_time.astimezone(local)
```


```python
print("UTC Time:",
      utc_time.strftime('%Y-%m-%d %H:%M:%S')
     )
print("Local Time (IST):",
      local_time.strftime('%Y-%m-%d %H:%M:%S')
     )
```

    UTC Time: 2024-11-26 16:48:29
    Local Time (IST): 2024-11-26 22:18:29



```python

```


---
**Score: 5**
