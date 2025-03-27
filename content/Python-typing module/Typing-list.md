---
title: Typing-List
date: 2025-03-27
author: Your Name
cell_count: 7
score: 5
---

```python
# Created at 19-03-2025
```


```python
# https://stevejoe1412.gitbook.io/ssn/python-subtopics/1.-typing-module - referance
```


```python
# List
```


```python
from typing import List
```


```python
def list_data(data: List[str]) -> str:
    for item in data:
        print(f"Name: {item}")
    if not item:
        print("Don't have more than two index")
```


```python
data = ['Alice','Bob']
list_data(data)
```

    Name: Alice
    Name: Bob



```python

```


---
**Score: 5**
