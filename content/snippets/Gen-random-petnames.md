---
title: Gen-Random-Petnames
date: 2024-12-02
author: Your Name
cell_count: 7
score: 5
---

```python
#import neccessery libraries
```


```python
import petname
```


```python
#create a method called ran_petname()
```


```python
def ran_petname():
    name = petname.generate(
        words=3,
        separator="_"
    )
    return name
```


```python
#set a range for the method
```


```python
for _ in range(5):
    print(ran_petname())
```

    lovely_cute_maggot
    newly_valued_swine
    rarely_tough_marmot
    solely_heroic_kite
    freely_ruling_fly



```python

```


---
**Score: 5**
