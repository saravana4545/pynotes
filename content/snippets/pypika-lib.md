---
title: Pypika-Lib
date: 2024-11-22
author: Your Name
cell_count: 5
score: 5
---

```python
from pypika import Query, Table
```


```python
def create_table(users):
    query = Query.from_(users).select("id", "name", "email")
    return query
def add_where_class(users):
    query = Query.from_(users).select("id", "name").where(users.name == "SARAVANA")
    return query
def insert_data(users):
    query = Query.into(users).columns("id", "name", "email").insert(1, "SARAVANA", "saro@example.com")
    return query
def update_data(users):
    query = Query.update(users).set(users.name, "andal").where(users.id == 1)
    return query
def delete_data(users):
    query = Query.from_(users).delete().where(users.name == "SARAVANA")
    return query
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
**Score: 5**