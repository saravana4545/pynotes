---
title: Beatifulsoup-Heading
date: 2024-12-05
author: Your Name
cell_count: 13
score: 10
---

```python
#1.Webpage Title Extraction
#Extract the title of a webpage from its HTML content.
```


```python
#import neccesery libraries
```


```python
from bs4 import BeautifulSoup
```


```python
import requests
```


```python
#put the url 
```


```python
url = "https://books.toscrape.com/catalogue/a-light-in-the-attic_1000/index.html"
```


```python
#get url using requests 
```


```python
response = requests.get(url)
```


```python
#parse the html content
```


```python
soup = BeautifulSoup(response.content, 'html.parser')
```


```python
#add the title
```


```python
title = soup.find('h1').text
print("Title tag:", title )
```

    Title tag: A Light in the Attic



```python

```


---
**Score: 10**
