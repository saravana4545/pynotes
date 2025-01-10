---
title: Update-Cityname
date: 2025-01-10
author: Your Name
cell_count: 5
score: 5
---

```python
class Person:
    def __init__(self, name, age, gender,city):
        self.name   = name
        self.age    = age
        self.gender = gender
        self.city   = city

    def intro(self, city):
        return f"Hi my name is {self.name} and my age is {self.age} and i am from {city}"
```


```python
class ChildPerson(Person):
    def __init__(self, name, age, gender, city):
        super().__init__(name, age, gender, city)

    def update_city(self, city):
        resul = super().intro(city)
        print(f"result is:{resul}")
        return resul
```


```python
result = ChildPerson(name= "saravana", age=20, gender="male", city="chennai")
```


```python
result.update_city(city="madurai")
```

    result is:Hi my name is saravana and my age is 20 and i am from madurai





    'Hi my name is saravana and my age is 20 and i am from madurai'




```python

```


---
**Score: 5**
