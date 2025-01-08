---
title: Selenium-With-Webdriver
date: 2025-01-08
author: Your Name
cell_count: 10
score: 10
---

```python
#Import neccessary libraries
```


```python
from selenium import webdriver
from selenium.webdriver.common.by import By
```


```python
# Set up the driver (e.g., ChromeDriver)
```


```python
driver = webdriver.Chrome()
driver.get("https://www.youtube.com")
```


```python
# Extract text
```


```python
heading = driver.find_element(By.TAG_NAME, "h1").text
print("Heading:", heading)
```


```python
# Extract attribute value
```


```python
link = driver.find_element(By.TAG_NAME, "a")
href = link.get_attribute("href")
print("Link URL:", href)
```


```python
#Quit from the entire browser
```


```python
driver.quit()
```


---
**Score: 10**
