---
title: Filehandling-Error
date: 2025-01-10
author: Your Name
cell_count: 10
score: 10
---

```python
# File Handling Inside a Method
```


```python

```


```python
def read_file(file_name):
    try:
        with open(file_name, "r") as file:
            return file.read()
    except FileNotFoundError:
        return f"Error: File '{file_name}' not found."
    except PermissionError:
        return f"Error: You don't have permission to read the file '{file_name}'."
```


```python
# Example Usage
```


```python

```


```python
# File exists
```


```python
print(read_file("example.txt")) 
```

    Error: File 'example.txt' not found.



```python
 # File not found
```


```python
print(read_file("nonexistent.txt"))
```

    Error: File 'nonexistent.txt' not found.



```python

```


---
**Score: 10**
