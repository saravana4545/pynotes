---
title: Find-Pattern-With-Re
date: 2024-11-26
author: Your Name
cell_count: 6
score: 5
---

```python
import re
```


```python
text = "Email me at example@gmail.com or support@example.org."
```


```python
pattern = r"[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}"
```


```python
matches = re.findall(pattern, text)
```


```python
for match in matches:
    print("Found email:", match)
```

    Found email: example@gmail.com
    Found email: support@example.org



```python

```


---
**Score: 5**
