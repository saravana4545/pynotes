---
title: Switch-Using-Operators
date: 2025-03-25
author: Your Name
cell_count: 12
score: 10
---

```python
# Created at 30-01-2025
```


```python
# https://www.scientecheasy.com/2022/11/switch-statement-in-python.html/
```


```python
# Switch Statement
```


```python
def add(a, b):
    return a + b
```


```python
def subtract(a, b):
    return a - b
```


```python
def multiply(a, b):
    return a * b
```


```python
def divide(a, b):
    return a / b 
```


```python
def default_case():
    return "Invalid operation"
```


```python
operation_dict = {
    'add': add,
    'subtract': subtract,
    'multiply': multiply,
    'divide': divide
}
```


```python
def perform_operation(a, b):
    return operation_dict.get(a, b)
```


```python
print(perform_operation(5, 3))
print(perform_operation(5, 3))  
print(perform_operation(5, 50))
print(perform_operation(10, 5)) 
```

    3
    3
    50
    5



```python

```


---
**Score: 10**
