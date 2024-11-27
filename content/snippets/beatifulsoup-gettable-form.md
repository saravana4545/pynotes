---
title: Beatifulsoup-Gettable-Form
date: 2024-11-27
author: Your Name
cell_count: 8
score: 5
---

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
soup = BeautifulSoup(response.text, "html.parser")
```


```python
price_element = soup.select_one("#content_inner > article > table")
```


```python
if price_element:
    print("Price:", price_element.text)
else:
    print("Price not found")
```

    Price: 
    
    UPCa897fe39b1053632
    
    
    Product TypeBooks
    
    
    Price (excl. tax)Â£51.77
    
    
    Price (incl. tax)Â£51.77
    
    
    TaxÂ£0.00
    
    
    Availability
    In stock (22 available)
    
    
    Number of reviews
    0
    
    



```python

```


---
**Score: 5**
