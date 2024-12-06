---
title: Else-And-Finaly
date: 2024-12-06
author: Your Name
cell_count: 11
score: 10
---

```python
#Using else and finally in Methods
```


```python
def process_number(number):
    try:
        result = 100 / number
    except ZeroDivisionError:
        return "Error: Cannot divide by zero."
    except TypeError:
        return "Error: Input must be a number."
    else:
        return f"Result: {result}" 
    finally:
        print("Method execution completed.") 
```


```python
# else Block: Executes if no exception occurs.
```


```python
# finally Block: Runs regardless of whether an exception occurred. Ideal for cleanup tasks.
```


```python
# Valid input
```


```python
print(process_number(5)) 
```

    Method execution completed.
    Result: 20.0



```python
 # Division by zero
```


```python
print(process_number(0)) 
```

    Method execution completed.
    Error: Cannot divide by zero.



```python
# Invalid input
```


```python
print(process_number("a")) 
```

    Method execution completed.
    Error: Input must be a number.



```python

```


---
**Score: 10**
