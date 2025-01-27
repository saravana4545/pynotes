---
title: Zero-Type-Erroe
date: 2025-01-27
author: Your Name
cell_count: 12
score: 10
---

```python
#Handling Errors in a Method
```


```python

```


```python
def divide_numbers(numerator, denominator):
    try:
        result = numerator / denominator
        return result
    except ZeroDivisionError:
        return "Error: Cannot divide by zero."
    except TypeError:
        return "Error: Both numerator and denominator must be numbers."
```


```python
# Example Usage
```


```python

```


```python
# Valid
```


```python
print(divide_numbers(10, 2)) 
```

    5.0



```python
# Division by zero
```


```python
print(divide_numbers(10, 0)) 
```

    Error: Cannot divide by zero.



```python
# Invalid type
```


```python
print(divide_numbers(10, "a")) 
```

    Error: Both numerator and denominator must be numbers.



```python

```


---
**Score: 10**
