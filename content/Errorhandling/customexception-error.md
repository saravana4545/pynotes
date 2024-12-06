---
title: Customexception-Error
date: 2024-12-06
author: Your Name
cell_count: 14
score: 10
---

```python
#Custom Exception Handling in Methods
```


```python

```


```python
class CustomError(Exception):
    pass
```


```python
#Demonstrates how to define and handle custom exceptions.
```


```python

```


```python
def validate_positive_number(number):
    try:
        if number < 0:
            raise CustomError("Number must be positive.")
        return f"Valid number: {number}"
    except CustomError as e:
        return f"Error: {e}"
```


```python

```


```python
# Example Usage
```


```python

```


```python
print(validate_positive_number(10))  # Valid
```

    Valid number: 10



```python
# Raises CustomError
```


```python

```


```python
print(validate_positive_number(-5)) 
```


```python

```


---
**Score: 10**
