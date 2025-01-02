---
title: Pypika-Lib
date: 2025-01-02
author: Your Name
cell_count: 17
score: 15
---

```python
#import neccessery libraries
```


```python
from pypika import Query, Table
```


```python
#This function generates a SQL-like SELECT query.
```


```python
def create_table(users):
    query = Query.from_(users).select("id", "name", "email")
    return query
```


```python
#This function generates a SELECT query with a WHERE condition.
```


```python
def add_where_class(users):
    query = Query.from_(users).select("id", "name").where(users.name == "SARAVANA")
    return query
```


```python
#This function generates an INSERT query.
```


```python
def insert_data(users):
    query = Query.into(users).columns("id", "name", "email").insert(1, "SARAVANA", "saro@example.com")
    return query
```


```python
#This function generates an UPDATE query.
```


```python
def update_data(users):
    query = Query.update(users).set(users.name, "andal").where(users.id == 1)
    return query
```


```python
#This function generates a DELETE query.
```


```python
def delete_data(users):
    query = Query.from_(users).delete().where(users.name == "SARAVANA")
    return query
```


```python
#create a method called startpy, where we can run the all above methods
```


```python
def startpy():
    print(create_table(Table("users")))
    print(add_where_class(Table("users")))
    print(insert_data(Table("users")))
    print(update_data(Table("users")))
    print(delete_data(Table("users")))
```


```python
#This line checks if the script is being run directly or imported
```


```python
if __name__ == '__main__':
    startpy()
```

    SELECT "id","name","email" FROM "users"
    SELECT "id","name" FROM "users" WHERE "name"='SARAVANA'
    INSERT INTO "users" ("id","name","email") VALUES (1,'SARAVANA','saro@example.com')
    UPDATE "users" SET "name"='andal' WHERE "id"=1
    DELETE FROM "users" WHERE "name"='SARAVANA'



```python

```


---
**Score: 15**
