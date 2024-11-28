---
title: Palindrom
date: 2024-11-28
author: Your Name
cell_count: 3
score: 0
---

```python
def is_palindrome(string):
    string = string.lower().replace(" ", "")
    return string == string[::-1]
```


```python
text = input("Enter a string: ")
if is_palindrome(text):
    print(f'"{text}" is a palindrome.')
else:
    print(f'"{text}" is not a palindrome.')
```

    Enter a string:  madam


    "madam" is a palindrome.



```python

```


---
**Score: 0**
