---
title: Palindrom
date: 2024-12-03
author: Your Name
cell_count: 5
score: 5
---

```python
#create a method called is_palindrome()
```


```python
def is_palindrome(string):
    string = string.lower().replace(" ", "")
    return string == string[::-1]
```


```python
#create a variable to get a value from user is palindrom or not.
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
**Score: 5**
