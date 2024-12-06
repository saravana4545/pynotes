---
title: Css-Selector
date: 2024-12-06
author: Your Name
cell_count: 7
score: 5
---

```python
#13. CSS Selector Usage
#Use CSS selectors with select() to scrape specific elements.
```


```python
from bs4 import BeautifulSoup
```


```python
html_content = """
<html>
<head>
    <title>Sample Page</title>
</head>
<body>
    <div class="content">
        <h1 class="title">Welcome to Web Scraping</h1>
        <p id="description">This page demonstrates web scraping using CSS selectors.</p>
        <ul class="items">
            <li class="item">Item 1</li>
            <li class="item">Item 2</li>
            <li class="item">Item 3</li>
        </ul>
    </div>
</body>
</html>
"""
```


```python
soup = BeautifulSoup(html_content, 'html.parser')
```


```python
title = soup.select('.title')[0].text
description = soup.select('#description')[0].text
items = [item.text for item in soup.select('.item')]
```


```python
print(f"Title: {title}")
print(f"Description: {description}")
print(f"Items: {items}")
```

    Title: Welcome to Web Scraping
    Description: This page demonstrates web scraping using CSS selectors.
    Items: ['Item 1', 'Item 2', 'Item 3']



```python

```


---
**Score: 5**
