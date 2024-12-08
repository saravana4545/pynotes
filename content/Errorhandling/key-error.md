---
title: Key-Error
date: 2024-12-08
author: Your Name
cell_count: 11
score: 10
---

```python
#Handling Dictionary Lookups
```


```python

```


```python
def get_value(dictionary, key):
    try:
        return dictionary[key]
    except KeyError:
        return f"Error: The key '{key}' does not exist."
```


```python
# Example Usage
```


```python
data = {"name": "Saravana", "age": 25}
```


```python

```


```python
# Key exists
```


```python
print(get_value(data, "name")) 
```

    Saravana



```python
# Key does not exist
```


```python
print(get_value(data, "email"))
```

    Error: The key 'email' does not exist.



```python

```


---
**Score: 10**
