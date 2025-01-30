---
title: Switch-Using-Dict
date: 2025-01-30
author: Your Name
cell_count: 8
score: 5
---

```python
# Created at 27-01-2025
```


```python
# https://www.scientecheasy.com/2022/11/switch-statement-in-python.html/
```


```python
# Switch Using Dictionary format
```


```python
days_dict = {
    1: "Monday",
    2: "Tuesday",
    3: "Wednesday",
    4: "Thursday",
    5: "Friday",
    6: "Saturday",
    7: "Sunday"
}
```


```python
def get_day(day):
    return days_dict.get(day, "Invalid day")
```


```python
print(get_day(5))
```

    Friday



```python
print(get_day(10))
```

    Invalid day



```python

```


---
**Score: 5**
