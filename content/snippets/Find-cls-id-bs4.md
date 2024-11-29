---
title: Find-Cls-Id-Bs4
date: 2024-11-29
author: Your Name
cell_count: 8
score: 5
---

```python
#8. Class and ID-Based Selection
#Extract content using specific classes or IDs from a webpage.
```


```python
from bs4 import BeautifulSoup
```


```python
# Example HTML content
html_content = """
<html>
    <body>
        <div id="main">
            <h1>Main Header</h1>
            <p class="description">This is the main content description.</p>
        </div>
        <div class="sidebar">
            <h2>Sidebar Header</h2>
            <p class="description">This is the sidebar description.</p>
        </div>
    </body>
</html>
"""
```


```python
soup = BeautifulSoup(html_content, 'html.parser')
```


```python
main_div = soup.find(id="main")
print("Content in 'main':")
print(main_div.text.strip())
```

    Content in 'main':
    Main Header
    This is the main content description.



```python
sidebar_div = soup.find('div', class_='sidebar')
print("\nContent in 'sidebar':")
print(sidebar_div.text.strip())
```

    
    Content in 'sidebar':
    Sidebar Header
    This is the sidebar description.



```python
description_paragraphs = soup.find_all('p', class_='description')
print("\nDescriptions:")
for para in description_paragraphs:
    print(para.text)
```

    
    Descriptions:
    This is the main content description.
    This is the sidebar description.



```python

```


---
**Score: 5**
