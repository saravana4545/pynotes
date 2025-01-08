---
title: Basic-Regex
date: 2025-01-08
author: Your Name
cell_count: 15
score: 15
---

```python
!pip install regex
```

    Requirement already satisfied: regex in /home/saravanakumar/miniconda3/envs/py12/lib/python3.12/site-packages (2024.11.6)



```python
#import neccessary libraries
```


```python
import re
```


```python
text = "The price is $20."
```


```python
# Search for a dollar amount
```


```python
match = re.search(r'\$\d+', text)
```


```python
# r'\$' matches the dollar symbol, '\d+' matches one or more digits
```


```python
if match:
    print("Found:", match.group())
```

    Found: $20



```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


```python

```


---
**Score: 15**
