---
title: Pandas-Crud
date: 2025-01-10
author: Your Name
cell_count: 16
score: 15
---

```python
#import neccessery libraries
```


```python
import pandas as pd
```


```python
#create a file and dump the datas
```


```python
def create_df(filename):
    data = {
        'name':['andal','saravana','santhosh','sandy'],
        'age':[25,26,27,28],
        'city':['chennai','madurai','coimbatore','salem']
    }
    df = pd.DataFrame(data)
    df.to_excel(
        filename,
        index=False
    )
```


```python
#read the excel file
```


```python
def read_excel(file_name):
    df = pd.read_excel(file_name)
    return df
```


```python
#update a new data on the excel file
```


```python
def update_df(file_name):
    #read dataframe
    df = pd.read_excel(file_name)
    df.loc[df['name']=='jerin','age'] = 21
    df.to_excel(
        file_name,
        index=False
    )
    return df
```


```python
#delete a some data in a excel file
```


```python
def delete_data_from_excel(file_name):
    df = pd.read_excel(file_name)
    dfs = df[df["name"]!= 'sanjay']
    dfs.to_excel(
        file_name,
        index=False
    )
    return dfs
```


```python
#create a method called startpy and call the all methods on that
```


```python
def startpy():
    print(create_df('example.xlsx'))
    print(read_excel('example.xlsx'))
    print(update_df('example.xlsx'))
    print(delete_data_from_excel('example.xlsx'))
```


```python
#This line checks if the script is being run directly or imported
```


```python
if __name__ == '__main__':
    startpy()
```

    None
           name  age        city
    0     andal   25     chennai
    1  saravana   26     madurai
    2  santhosh   27  coimbatore
    3     sandy   28       salem
           name  age        city
    0     andal   25     chennai
    1  saravana   26     madurai
    2  santhosh   27  coimbatore
    3     sandy   28       salem
           name  age        city
    0     andal   25     chennai
    1  saravana   26     madurai
    2  santhosh   27  coimbatore
    3     sandy   28       salem



```python

```


```python

```


---
**Score: 15**
