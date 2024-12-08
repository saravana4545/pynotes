---
title: Fake-Pattern(-)
date: 2024-12-08
author: Your Name
cell_count: 9
score: 5
---

```python
#import neccessery libraries
```


```python
from faker import Faker
```


```python
#connect the faker 
```


```python
fake = Faker()
```


```python
#create a method called address_pat()
```


```python
def address_pat():
    fak_address = fake.address()
    address = fak_address.replace(" ", "-")
    return address
```


```python
#set the range
```


```python
for _ in range(2):
    print(address_pat())
```

    881-Cynthia-Summit
    Port-Paulabury,-OR-66193
    34627-Thompson-Glen-Suite-767
    Hayleystad,-ND-50275



```python

```


---
**Score: 5**
