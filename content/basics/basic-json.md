---
title: Basic-Json
date: 2025-01-25
author: Your Name
cell_count: 5
score: 5
---

```python
import json
```


```python
class City:
    def toJSON(self):
        return json.dumps(self, default=lambda o: o.__dict__, sort_keys=True, indent=4)
```


```python
me = City()
me.name = "Onur"
me.id = 1

print(me.toJSON()) 
```

    {
        "id": 1,
        "name": "Onur"
    }



```python

```


```python

```


---
**Score: 5**
