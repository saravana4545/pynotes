---
title: Match-Method-Re
date: 2025-01-25
author: Your Name
cell_count: 12
score: 10
---

```python
#import re module
```


```python
import re
```


```python
#create a variable and put some text
```


```python
fruits = "apple, banana; orange: grape"
```


```python
# Match if the string starts with 'Python'
```


```python
match = re.match(r'apple', text)
```


```python
#check it's matched or not
```


```python
if match:
    print("Matched:", match.group())
```

    Matched: apple



```python
# Find '[;,:]' matches any of these characters using split()
```


```python
fruits = re.split(r'[;,:]', text)
```


```python
print("Fruits:", fruits)
```

    Fruits: ['apple', ' banana', ' orange', ' grape']



```python

```


---
**Score: 10**
