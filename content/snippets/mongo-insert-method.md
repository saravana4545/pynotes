---
title: Mongo-Insert-Method
date: 2024-12-02
author: Your Name
cell_count: 5
score: 5
---

```python
import pymongo
```


```python
myclient = pymongo.MongoClient("mongodb+srv://saravana45454:kumar123@saravana.kg1trkw.mongodb.net")
DB_NAME = myclient["mydatabase"]
DB_COL = DB_NAME["customers"]
```


```python
def data_add():
    mylist = [
      { "name": "Amy", "address": "Apple st 652"},
      { "name": "Hannah", "address": "Mountain 21"},
      { "name": "Michael", "address": "Valley 345"},
      { "name": "Sandy", "address": "Ocean blvd 2"}
    ]
    result = DB_COL.insert_many(mylist)
    return f"Data added successfully in {result}"
```


```python
print(data_add())
```

    Data added successfully in InsertManyResult([ObjectId('673f6a276605e9b22fc68ed3'), ObjectId('673f6a276605e9b22fc68ed4'), ObjectId('673f6a276605e9b22fc68ed5'), ObjectId('673f6a276605e9b22fc68ed6')], acknowledged=True)



```python

```


---
**Score: 5**
