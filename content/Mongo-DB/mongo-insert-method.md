---
title: Mongo-Insert-Method
date: 2024-12-09
author: Your Name
cell_count: 11
score: 10
---

```python
#import neccessary library
```


```python
from pymongo import MongoClient
```


```python
# Connect to MongoDB
```


```python
client       = MongoClient("mongodb+srv://saravana45454:kumar123@saravana.kg1trkw.mongodb.net")
db           = client["mydatabase"]
collection   = db["customers"]
```


```python

```


```python
#create a method called data_add() and give some datas
```


```python
def data_add():
    mylist = [
      { "name": "Amy",    "address": "Apple st 652"},
      { "name": "Hannah", "address": "Mountain 21"},
      { "name": "Michael","address": "Valley 345"},
      { "name": "Sandy",  "address": "Ocean blvd 2"}
    ]
    result = collection.insert_many(mylist)
    return f"Data added successfully in {result}"
```


```python

```


```python
#call the method inside print() 
```


```python
print(data_add())
```

    Data added successfully in InsertManyResult([ObjectId('67532025bf60b417069b9e34'), ObjectId('67532025bf60b417069b9e35'), ObjectId('67532025bf60b417069b9e36'), ObjectId('67532025bf60b417069b9e37')], acknowledged=True)



```python

```


---
**Score: 10**
