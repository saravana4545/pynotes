---
title: Getdetails-Usingbs4
date: 2024-12-02
author: Your Name
cell_count: 13
score: 10
---

```python
#import neccessery libraries
```


```python
import requests
from bs4 import BeautifulSoup
```


```python
# URL of the webpage to scrape
```


```python
url = "https://books.toscrape.com/catalogue/sapiens-a-brief-history-of-humankind_996/index.html"
```


```python
# Fetch the HTML content of the webpage
```


```python
response = requests.get(url)
```


```python
# Check if the request was successful
```


```python
if response.status_code == 200:
    soup = BeautifulSoup(response.text, 'html.parser')
```


```python
# Extract book details
```


```python
    books = soup.find_all('article', class_='product_pod')
    for book in books:
        # Extract book title
        title = book.h3.a['title']
        
        # Extract book price
        price = book.find('p', class_='price_color').text
        
        # Extract book link (relative URL)
        link = book.h3.a['href']
        full_link = f"https://books.toscrape.com/catalogue/{link}"
        
        print(f"Title: {title}")
        print(f"Price: {price}")
        print(f"Link: {full_link}")
        print("-" * 40)

```

    Title: Sharp Objects
    Price: Â£47.82
    Link: https://books.toscrape.com/catalogue/../sharp-objects_997/index.html
    ----------------------------------------
    Title: Soumission
    Price: Â£50.10
    Link: https://books.toscrape.com/catalogue/../soumission_998/index.html
    ----------------------------------------
    Title: Tipping the Velvet
    Price: Â£53.74
    Link: https://books.toscrape.com/catalogue/../tipping-the-velvet_999/index.html
    ----------------------------------------
    Title: A Light in the Attic
    Price: Â£51.77
    Link: https://books.toscrape.com/catalogue/../a-light-in-the-attic_1000/index.html
    ----------------------------------------



```python
#check when the request was fail else will be run
```


```python
else:
    print(f"Failed to retrieve the webpage. Status code: {response.status_code}")
```


```python

```


---
**Score: 10**
