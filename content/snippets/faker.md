---
title: Faker
date: 2025-01-30
author: Your Name
cell_count: 9
score: 5
---

```python
#import the faker module
```


```python
from faker import Faker
```


```python
#call the Faker module using variable
```


```python
fake = Faker()
```


```python
#create a method called fake_detailes
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
