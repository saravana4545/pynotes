---
title: Bs4-Basic
date: 2025-01-30
author: Your Name
cell_count: 11
score: 10
---

```python
#import neccessary libraries
```


```python
from bs4 import BeautifulSoup
```


```python
#create html content
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
#parse the html content
```


```python
soup = BeautifulSoup(html_content, 'html.parser')
```


```python
#print the title
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
**Score: 10**
