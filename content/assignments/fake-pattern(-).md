---
title: Fake-Pattern(-)
date: 2024-11-28
author: Your Name
cell_count: 5
score: 5
---

```python
from faker import Faker
```


```python
fake = Faker()
```


```python
def address_pat():
    fak_address = fake.address()
    address = fak_address.replace(" ", "-")
    return address
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
