---
title: Collections-Lib
date: 2024-11-26
author: Your Name
cell_count: 5
score: 5
---

```python
from collections import Counter, defaultdict, deque
```


```python
# Counter example
data = ['apple', 'banana', 'apple', 'orange', 'banana', 'apple']
counter = Counter(data)
print("Counts:", counter)
```

    Counts: Counter({'apple': 3, 'banana': 2, 'orange': 1})



```python
# defaultdict example
scores = defaultdict(list)
scores['Alice'].append(90)
scores['Bob'].append(85)
print("Scores:", dict(scores))
```

    Scores: {'Alice': [90], 'Bob': [85]}



```python
# deque example
queue = deque([1, 2, 3])
queue.append(4)
queue.popleft()
print("Deque:", queue)
```

    Deque: deque([2, 3, 4])



```python

```


---
**Score: 5**
