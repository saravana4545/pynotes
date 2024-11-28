---
title: Bs4-Basic
date: 2024-11-28
author: Your Name
cell_count: 7
score: 5
---

```python
from bs4 import BeautifulSoup
```


```python
html_content = """
<html>
    <head><title>My Web Page</title></head>
    <body>
        <h1>Welcome to Web Scraping</h1>
        <p>This is a <b>simple</b> example.</p>
    </body>
</html>
"""
```


```python
soup = BeautifulSoup(html_content, 'html.parser')
```


```python
print(soup.title.string)
```

    My Web Page



```python
print(soup.h1.text)
```

    Welcome to Web Scraping



```python
print(soup.p.text)
```

    This is a simple example.



```python

```


---
**Score: 5**