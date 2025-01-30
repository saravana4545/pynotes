---
title: Collections-Lib
date: 2025-01-30
author: Your Name
cell_count: 10
score: 10
---

```python
#import collections library
```


```python
# !pip install collections like this
```


```python
from collections import Counter, defaultdict, deque
```


```python
# Counter example
```


```python
data = ['apple', 'banana', 'apple', 'orange', 'banana', 'apple']
counter = Counter(data)
print("Counts:", counter)
```

    Counts: Counter({'apple': 3, 'banana': 2, 'orange': 1})



```python
# defaultdict example
```


```python
scores = defaultdict(list)
scores['Alice'].append(90)
scores['Bob'].append(85)
print("Scores:", dict(scores))
```

    Scores: {'Alice': [90], 'Bob': [85]}



```python
# deque example
```


```python
queue = deque([1, 2, 3])
queue.append(4)
queue.popleft()
print("Deque:", queue)
```

    Deque: deque([2, 3, 4])



```python

```


---
**Score: 10**
