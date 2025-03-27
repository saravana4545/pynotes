---
title: Generate-Fake-Name
date: 2025-03-27
author: Your Name
cell_count: 11
score: 10
---

```python
#created at 08-01-2025.
```


```python
#import neccesary libraries
```


```python
from faker import Faker
```


```python
fake=Faker()
```


```python
# create a method like generate_random_names().
```


```python
def generate_random_names():
    random_names = []
    for x in range(5) :
        random_names.append(fake.name())
    return  random_names
```


```python
# create a method like startpy() and call the above method inside of here..
```


```python
def startpy():
    random_name_list = generate_random_names()   
    print(random_name_list)
```


```python
# And call the main method here
```


```python
if __name__ == '__main__':
    startpy()
```

    ['John Cannon', 'Amy Anthony', 'Raymond Robinson', 'Eric Hansen', 'Leslie Cook']



```python

```


---
**Score: 10**
