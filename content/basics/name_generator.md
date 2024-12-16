---
title: Name Generator
date: 2024-12-16
author: Your Name
cell_count: 7
score: 5
---

```python
import namegenerator
```


```python
import uuid
```


```python
def name_gen():
    random_name = namegenerator.gen()
    return random_name
```


```python
def unique_id():
    random_name = namegenerator.gen()
    unique_name = f"{random_name}-{uuid.uuid4().hex[:8]}"
    return unique_name
```


```python
def startpy():
    print(name_gen())
    print(unique_id())
```


```python
if __name__ == '__main__':
    startpy()
```

    sleepy-lilac-gerbil
    hasty-orchid-crab-fb050e54



```python

```


---
**Score: 5**
