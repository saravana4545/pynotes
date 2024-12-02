---
title: Capturing-Group-Using-Re
date: 2024-12-02
author: Your Name
cell_count: 8
score: 5
---

```python
#import re module
```


```python
import re
```


```python
#Using Parentheses () for Capturing Groups
```


```python
text = "My phone number is 123-456-7890."
```


```python
# Extract the area code and number
```


```python
match = re.search(r'(\d{3})-(\d{3})-(\d{4})', text)
```


```python
if match:
    print("Full Match:", match.group())  # Output: 123-456-7890
    print("Area Code:", match.group(1))  # Output: 123
    print("First 3 Digits:", match.group(2))  # Output: 456
    print("Last 4 Digits:", match.group(3))  # Output: 7890
```

    Full Match: 123-456-7890
    Area Code: 123
    First 3 Digits: 456
    Last 4 Digits: 7890



```python

```


---
**Score: 5**
