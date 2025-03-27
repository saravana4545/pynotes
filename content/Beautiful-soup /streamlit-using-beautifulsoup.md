---
title: Streamlit-Using-Beautifulsoup
date: 2025-03-27
author: Your Name
cell_count: 13
score: 10
---

```python
#import neccesary libraries
```


```python
import streamlit as st
from urllib.parse import urlparse
from bs4 import BeautifulSoup
import requests
```


```python
# we can use it for to create a title in webpage
```


```python
st.title("School ID Extractor")
```


```python
# we can use it for text inside of the search box
```


```python
url = st.text_input("Enter the school URL :")
```


```python
# create a method called get_data(),
```


```python
def get_data()
    if st.button("Extarct ID"):
        try:
            get_url = urlparse(url)
            path_parts = get_url.path.split('/')
    
            if path_parts:
                response = requests.get(url)
                
                if response.status_code == 200:
                    
                    soup = BeautifulSoup(response.content, 'html.parser')
                    
                    data = soup.select_one('#main_div > div:nth-child(2) > div:nth-child(1)')
                    
                    if data:
                        st.info(f"School code : {data.text.strip()}")
                    else:
                        st.warning ("No content found using the specified CSS selector.")
                else:
                    st.error(f"Failed to fetch the webpage. HTTP Status Code :{response.status_code}")
                    
        except Exception as e :
            st.error (f"Error: {e}")
```


```python
# create a var and call the method inside.
```


```python
result = get_data()
```

    <function get_data at 0x7fee13f83ba0>



```python
#  print the var 
```


```python
print(result)
```


```python

```


---
**Score: 10**
