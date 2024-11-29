---
title: Beatifulsoup-Heading
date: 2024-11-29
author: Your Name
cell_count: 8
score: 5
---

```python
#1.Webpage Title Extraction
#Extract the title of a webpage from its HTML content.
```


```python
from bs4 import BeautifulSoup
```


```python
import requests
```


```python
url = "https://books.toscrape.com/catalogue/a-light-in-the-attic_1000/index.html"
```


```python
response = requests.get(url)
```


```python
soup = BeautifulSoup(response.content, 'html.parser')
```


```python
title = soup.find('h1').text
print("Title tag:", title )
```

    Title tag: A Light in the Attic



```python

```


---
**Score: 5**
