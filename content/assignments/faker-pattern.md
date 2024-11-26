---
title: Faker-Pattern
date: 2024-11-26
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
    address = fak_address.replace(" ", "/")
    return address
```


```python
for _ in range(2):
    print(address_pat())
```

    3946/Braun/Hill/Apt./495
    North/Kathleen,/LA/91986
    05851/Maria/Lodge/Suite/728
    Teresamouth,/WA/02644



```python

```


---
**Score: 5**
