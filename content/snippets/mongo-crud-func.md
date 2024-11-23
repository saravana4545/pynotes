---
title: Mongo-Crud-Func
date: 2024-11-23
author: Your Name
cell_count: 5
score: 5
---

```python
from pymongo import MongoClient
```


```python
# Connect to MongoDB
client = MongoClient("mongodb+srv://saravana45454:kumar123@saravana.kg1trkw.mongodb.net")
db = client["test_db"] 
collection = db["session_1"]
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

def read_documents():
    print("\nReading Documents:")
    for doc in collection.find():
        print(doc)
        
def update_document():
    filter_criteria = {"name": "Alice"}
    new_values = {"$set": {"age": 26, "skills": ["Python", "Django", "MongoDB"]}}
    result = collection.update_one(filter_criteria, new_values)
    print("Matched Count:", result.matched_count, "Modified Count:", result.modified_count)

def delete_document():
    filter_criteria = {"name": "Alice"}
    result = collection.delete_one(filter_criteria)
    print("Deleted Count:", result.deleted_count)
```


```python
if __name__ == "__main__":
    create_document() 
    read_documents() 
    update_document()
    delete_document() 
```

    Inserted Document ID: 674207f584134f2a7672d82e
    
    Reading Documents:
    {'_id': ObjectId('674207f584134f2a7672d82e'), 'name': 'Alice', 'age': 25, 'skills': ['Python', 'Flask', 'MongoDB']}
    Matched Count: 1 Modified Count: 1
    Deleted Count: 1



```python

```


---
**Score: 5**
