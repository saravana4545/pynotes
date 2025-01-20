---
title: Findpass-Hashlib
date: 2025-01-20
author: Your Name
cell_count: 14
score: 10
---

```python
#Import neccessary module
```


```python
import hashlib
```


```python
# Original password
```


```python
password = "Saro@2003"
```


```python
# Hash the password
```


```python
hashed_password = hashlib.sha256(password.encode()).hexdigest()
```


```python
# Simulate user input and hash it
```


```python
user_input = "Saro@2003"
hashed_input = hashlib.sha256(user_input.encode()).hexdigest()
```


```python
# Compare hashes
```


```python
if hashed_password == hashed_input:
    print("Password match!")
else:
    print("Incorrect password.")
```

    Password match!



```python

```


```python

```


```python

```


```python

```


---
**Score: 10**
