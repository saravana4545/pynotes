---
title: Typing-Typeddict
date: 2025-03-25
author: Your Name
cell_count: 8
score: 5
---

```python
# Created at 19-03-2025
```


```python
# https://stevejoe1412.gitbook.io/ssn/python-subtopics/1.-typing-module - referance
```


```python
# TypedDict method
```


```python
from typing import TypedDict
```


```python
class Person(TypedDict):
    name: str
    age: int
```


```python
def display_person(person: Person) -> None:
    print(f"Name: {person['name']}, Age: {person['age']}")
```


```python
person = {'name': 'Alice', 'age': 25}
display_person(person)
```

    Name: Alice, Age: 25



```python

```


---
**Score: 5**
