---
title: Mongo-Crud-Func
date: 2024-12-23
author: Your Name
cell_count: 16
score: 15
---

```python
#import neccessary libraries
```


```python
from pymongo import MongoClient
```


```python
# Connect to MongoDB
```


```python
client     = MongoClient("mongodb+srv://saravana45454:kumar123@saravana.kg1trkw.mongodb.net")
db         = client["test_db"] 
collection = db["session_1"]
```


```python
#create a method called create_document() 
```


```python
def create_document():
    new_document = {
        "name": "Alice",
        "age": 25,
        "skills": ["Python", "Flask", "MongoDB"]
    }
    result = collection.insert_one(new_document)
    print("Inserted Document ID:", result.inserted_id)
```


```python
#create a method for Read the documents
```


```python
def read_documents():
    print("\nReading Documents:")
    for doc in collection.find():
        print(doc)
```


```python
#create a method for update the documents
```


```python
def update_document():
    filter_criteria = {"name": "Alice"}
    new_values = {"$set": {"age": 26, "skills": ["Python", "Django", "MongoDB"]}}
    result = collection.update_one(filter_criteria, new_values)
    print("Matched Count:", result.matched_count, "Modified Count:", result.modified_count)
```


```python
#create a method for delete the documents
```


```python
def delete_document():
    filter_criteria = {"name": "Alice"}
    result = collection.delete_one(filter_criteria)
    print("Deleted Count:", result.deleted_count)
```


```python
#create a method called startpy() and here we can call the all methods
```


```python
def startpy():
    create_document() 
    read_documents() 
    update_document()
    delete_document()
```


```python
if __name__ == "__main__":
     startpy()
```

    Inserted Document ID: 6753200d2595f81b5f9fd86f
    
    Reading Documents:
    {'_id': ObjectId('6753200d2595f81b5f9fd86f'), 'name': 'Alice', 'age': 25, 'skills': ['Python', 'Flask', 'MongoDB']}
    Matched Count: 1 Modified Count: 1
    Deleted Count: 1



```python

```


---
**Score: 15**
