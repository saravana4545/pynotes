---
title: Selenium-Basic
date: 2024-12-05
author: Your Name
cell_count: 13
score: 10
---

```python
#Import neccessary libraries
```


```python
!pip install selenium
```

    Requirement already satisfied: selenium in /home/saravanakumar/miniconda3/envs/py12/lib/python3.12/site-packages (4.27.1)
    Requirement already satisfied: urllib3<3,>=1.26 in /home/saravanakumar/miniconda3/envs/py12/lib/python3.12/site-packages (from urllib3[socks]<3,>=1.26->selenium) (2.2.3)
    Requirement already satisfied: trio~=0.17 in /home/saravanakumar/miniconda3/envs/py12/lib/python3.12/site-packages (from selenium) (0.27.0)
    Requirement already satisfied: trio-websocket~=0.9 in /home/saravanakumar/miniconda3/envs/py12/lib/python3.12/site-packages (from selenium) (0.11.1)
    Requirement already satisfied: certifi>=2021.10.8 in /home/saravanakumar/miniconda3/envs/py12/lib/python3.12/site-packages (from selenium) (2024.8.30)
    Requirement already satisfied: typing_extensions~=4.9 in /home/saravanakumar/miniconda3/envs/py12/lib/python3.12/site-packages (from selenium) (4.12.2)
    Requirement already satisfied: websocket-client~=1.8 in /home/saravanakumar/miniconda3/envs/py12/lib/python3.12/site-packages (from selenium) (1.8.0)
    Requirement already satisfied: attrs>=23.2.0 in /home/saravanakumar/miniconda3/envs/py12/lib/python3.12/site-packages (from trio~=0.17->selenium) (24.2.0)
    Requirement already satisfied: sortedcontainers in /home/saravanakumar/miniconda3/envs/py12/lib/python3.12/site-packages (from trio~=0.17->selenium) (2.4.0)
    Requirement already satisfied: idna in /home/saravanakumar/miniconda3/envs/py12/lib/python3.12/site-packages (from trio~=0.17->selenium) (3.10)
    Requirement already satisfied: outcome in /home/saravanakumar/miniconda3/envs/py12/lib/python3.12/site-packages (from trio~=0.17->selenium) (1.3.0.post0)
    Requirement already satisfied: sniffio>=1.3.0 in /home/saravanakumar/miniconda3/envs/py12/lib/python3.12/site-packages (from trio~=0.17->selenium) (1.3.1)
    Requirement already satisfied: wsproto>=0.14 in /home/saravanakumar/miniconda3/envs/py12/lib/python3.12/site-packages (from trio-websocket~=0.9->selenium) (1.2.0)
    Requirement already satisfied: pysocks!=1.5.7,<2.0,>=1.5.6 in /home/saravanakumar/miniconda3/envs/py12/lib/python3.12/site-packages (from urllib3[socks]<3,>=1.26->selenium) (1.7.1)
    Requirement already satisfied: h11<1,>=0.9.0 in /home/saravanakumar/miniconda3/envs/py12/lib/python3.12/site-packages (from wsproto>=0.14->trio-websocket~=0.9->selenium) (0.14.0)



```python
from selenium import webdriver
```


```python
# Set up the driver (e.g., ChromeDriver)
```


```python
driver = webdriver.Firefox()
```


```python
# Open a webpage
```


```python
driver.get("https://www.youtube.com")
```


```python
# Print the title of the webpage
```


```python
print("Page title:", driver.title)
```

    Page title: YouTube



```python
# Close the browser
```


```python
driver.quit()
```


```python

```


```python

```


---
**Score: 10**
