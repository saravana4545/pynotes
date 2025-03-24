---
title: Form-Data-Extraction
date: 2025-03-24
author: Your Name
cell_count: 8
score: 5
---

```python
#10. Form Data Extraction
#Extract all form elements (<form>, <input>, <button>) from a webpage.
```


```python
from bs4 import BeautifulSoup
```


```python
html_content = """
<html>
    <body>
        <form action="/submit" method="post">
            <label for="username">Username:</label>
            <input type="text" id="username" name="username">
            
            <label for="password">Password:</label>
            <input type="password" id="password" name="password">
            
            <input type="hidden" name="csrf_token" value="123456">
            
            <button type="submit">Login</button>
        </form>
    </body>
</html>
"""
```


```python
soup = BeautifulSoup(html_content, 'html.parser')
```


```python
form = soup.find('form')
print("Form Details:")
print(f"Action: {form.get('action')}")
print(f"Method: {form.get('method')}")
```

    Form Details:
    Action: /submit
    Method: post



```python
inputs = form.find_all('input')
print("\nInput Fields:")
for input_tag in inputs:
    print(f"Name: {input_tag.get('name')}, Type: {input_tag.get('type')}, id: {input_tag.get('id')}, value: {input_tag.get('value')}")
```

    
    Input Fields:
    Name: username, Type: text, id: username, value: None
    Name: password, Type: password, id: password, value: None
    Name: csrf_token, Type: hidden, id: None, value: 123456



```python
buttons = form.find_all('button')
print("\nButtons:")
for button in buttons:
    print(f"Type: {button.get('type')}, Text: {button.text}")
```

    
    Buttons:
    Type: submit, Text: Login



```python

```


---
**Score: 5**
