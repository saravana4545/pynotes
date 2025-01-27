---
title: Getting-Sch-Details
date: 2025-01-27
author: Your Name
cell_count: 17
score: 15
---

```python
# Using beautiful_soup and get details from url
```


```python
#import neccesary libraries
```


```python
from bs4 import BeautifulSoup
import requests
import pandas as pd
```


```python
#create a csv file and put inside variable
```


```python
filename = "school_details.csv"
```


```python
# we want a url
```


```python
url = "https://stackschools.com/schools/33120100909/air-force-schoolcoimbatore"
```


```python
response = requests.get(url)
```


```python
soup = BeautifulSoup(response.text, "html.parser")
```


```python
# create a method called get_data().
```


```python
def get_data():
    get_Code        = soup.select_one("#main_div > div:nth-child(2) > div:nth-child(1) > p > span")
    get_scl_name    = soup.select_one("#main_div > h2")
    publish_year    = soup.select_one("#main_div > div:nth-child(2) > div:nth-child(2) > p > span")
    Total_teachers  = soup.select_one("#main_div > div:nth-child(10) > p > span.badge.bg-info")
    Total_student   = soup.select_one("#main_div > div:nth-child(10) > p > span.badge.bg-danger")
    Total_classroom = soup.select_one("#main_div > div:nth-child(14) > p > span.badge.bg-warning")


    # if get_Code:
    #     print(get_Code.text)
    # else:
    #     print("UDISE Code is not found")

    data = {
        "school_name"     : get_scl_name.text,
        "school_code"     : get_Code.text,
        "publish_year"    : publish_year.text,
	    "Total_teachers"  : Total_teachers.text,
	    "Total_student"   : Total_student.text,
	    "Total_classroom" : Total_classroom.text
    }

    df = pd.DataFrame([data])
    df.to_csv(filename, mode='a', index=False)

    return df
```


```python
# create variable for the method.
```


```python
result = get_data()
```


```python
# print the variable 
```


```python
print(result)
```

                       school_name  school_code publish_year Total_teachers  \
    0  AIR FORCE SCHOOL,COIMBATORE  33120100909         1952             26   
    
      Total_student Total_classroom  
    0           864              24  



```python

```


```python

```


---
**Score: 15**
