---
title: Convert-Int-As-Str
date: 2025-01-21
author: Your Name
cell_count: 7
score: 5
---

```python
#https://stackoverflow.com/questions/7368789/convert-all-strings-in-a-list-to-integers
```


```python
# 22- Write a function to convert a list of integers to a list of strings.
```


```python
def convert_integers_to_strings(lst):
    """
    Converts a list of integers to a list of strings.

    Parameters:
    lst (list): A list of integers to be converted.

    Returns:
    list: A list of strings converted from the integers.
    """
    # TODO: Complete the implementation of this function
    convert_list_as_str = [str(item) for item in lst]
    return convert_list_as_str
```


```python
# Sample test cases
```


```python
print(convert_integers_to_strings([1, 2, 3]))  # Expected output: ['1', '2', '3']
```

    ['1', '2', '3']



```python
print(convert_integers_to_strings([10, 20, 30]))  # Expected output: ['10', '20', '30']

```

    ['10', '20', '30']



```python

```


---
**Score: 5**
