---
title: Mergeing-List
date: 2025-01-25
author: Your Name
cell_count: 8
score: 5
---

```python
# created at: 08-01-2025 
```


```python
# merge two list using method.
```


```python
def get_merged_list(list1, list2):
    non_duplicates = []
    merged_list = list1 + list2
    for x in merged_list:
        if x not in non_duplicates:
            non_duplicates.append(x)
    return non_duplicates
```


```python
# create lists in method.
```


```python
def lists():
    list1 = [
        "jupiter",
        "prakash",
        "ram",
        "raju",
        "bruno",
        2.3
    ]
    list2 = [
        2.3,
        "jupiter",
        "mars",
        "mercury",
        "venus",
        134340,
        "saturn"
    ]
    combined_list = get_merged_list(list1, list2)   
    print(combined_list)
```


```python
# call the method here...
```


```python
lists()
```

    ['jupiter', 'prakash', 'ram', 'raju', 'bruno', 2.3, 'mars', 'mercury', 'venus', 134340, 'saturn']



```python

```


---
**Score: 5**
