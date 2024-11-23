---
title: Faker
date: 2024-11-23
author: Your Name
cell_count: 6
score: 5
---

```python
from faker import Faker
```


```python
fake = Faker()
```


```python
def fake_details():
    list = {
        "name"    : fake.name(),
        "address" : fake.address(),
        "emali"   : fake.email()
    }
    return list
```


```python
def startpy():
    print(fake_details())
```


```python
if __name__ == '__main__':
    startpy()
```

    {'name': 'Rebecca Soto', 'address': '24033 Matthew Canyon\nKaitlinmouth, MI 26633', 'emali': 'gordondiana@example.com'}



```python

```


---
**Score: 5**
