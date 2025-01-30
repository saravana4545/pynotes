---
title: Faker-Pattern
date: 2025-01-30
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
    address = fak_address.replace(" ", "/")
    return address
```


```python
#set the range
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
