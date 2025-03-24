---
title: Typing-Dict,Optional
date: 2025-03-24
author: Your Name
cell_count: 9
score: 5
---

```python
# Created at 19-03-2025
```


```python
# https://stevejoe1412.gitbook.io/ssn/python-subtopics/1.-typing-module - referance
```


```python
# Dict & Optional
```


```python
from typing import Dict, Optional
```


```python
def get_value(data: Dict[str, int], key: str) -> Optional[int]:
    return data.get(key)
```


```python
data = {'apple': 10, 'banana': 5}
```


```python
print(get_value(data, 'apple'))
```

    10



```python
print(get_value(data, 'grapes'))
```

    None



```python

```


---
**Score: 5**
