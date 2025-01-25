---
title: Samename-As-Global-Var
date: 2025-01-25
author: Your Name
cell_count: 7
score: 5
---

```python
# Created at 20-01-2025
```


```python
# https://www.scientecheasy.com/2022/09/global-and-local-variables-in-python.html/
```


```python
# create a variable inside a function with the same name as the global variable.
```


```python
name = "saravana"
```


```python
def same_var():
    name = "saravana" + "kumar"
    print("My full name is", name)
```


```python
same_var()
print("using global var outside", '-', name)
```

    My full name is saravanakumar
    using global var outside - saravana



```python

```


---
**Score: 5**
