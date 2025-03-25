---
title: Sql-Crud
date: 2025-03-25
author: Your Name
cell_count: 24
score: 20
---

```python
#import neccessary libraries
```


```python
import sqlite3
```


```python
# Establish database connection
```


```python
def connect():
    return sqlite3.connect("example.db")
```


```python
# Create Table (Run this once)
```


```python
def create_table():
    with connect() as conn:
        cursor = conn.cursor()
        cursor.execute("""
            CREATE TABLE IF NOT EXISTS users (
                id INTEGER PRIMARY KEY AUTOINCREMENT,
                name TEXT NOT NULL,
                age INTEGER NOT NULL,
                email TEXT UNIQUE NOT NULL
            )
        """)
        conn.commit()
```


```python
# CREATE
```


```python
def create_user(name, age, email):
    with connect() as conn:
        cursor = conn.cursor()
        cursor.execute("INSERT INTO users (name, age, email) VALUES (?, ?, ?)", (name, age, email))
        conn.commit()
        print("User added successfully!")
```


```python
# READ
```


```python
def get_users():
    with connect() as conn:
        cursor = conn.cursor()
        cursor.execute("SELECT * FROM users")
        rows = cursor.fetchall()
        for row in rows:
            print(row)
```


```python
# UPDATE
```


```python
def update_user(user_id, name=None, age=None, email=None):
    with connect() as conn:
        cursor = conn.cursor()
        updates = []
        if name:
            updates.append(f"name = '{name}'")
        if age:
            updates.append(f"age = {age}")
        if email:
            updates.append(f"email = '{email}'")
        if updates:
            query = f"UPDATE users SET {', '.join(updates)} WHERE id = ?"
            cursor.execute(query, (user_id,))
            conn.commit()
            print("User updated successfully!")
```


```python
# DELETE
```


```python
def delete_user(user_id):
    with connect() as conn:
        cursor = conn.cursor()
        cursor.execute("DELETE FROM users WHERE id = ?", (user_id,))
        conn.commit()
        print("User deleted successfully!")

```


```python
# Example Usage
```


```python
if __name__ == "__main__":
    create_table()
    
    # CREATE
    create_user("Alice", 25, "alice@example.com")
    create_user("Bob", 30, "bob@example.com")
    
```

    User added successfully!
    User added successfully!



```python
# READ
```


```python
    print("\nAll Users:")
    get_users()
    
  
```

    
    All Users:
    (1, 'Alice', 25, 'alice@example.com')
    (2, 'Bob', 30, 'bob@example.com')



```python
  # UPDATE
```


```python

    print("\nUpdating Bob's age:")
    update_user(2, age=35)
    get_users()
    

```

    
    Updating Bob's age:
    User updated successfully!
    (1, 'Alice', 25, 'alice@example.com')
    (2, 'Bob', 35, 'bob@example.com')



```python
 # DELETE
```


```python
   
    print("\nDeleting Alice:")
    delete_user(1)
    get_users()
```

    
    Deleting Alice:
    User deleted successfully!
    (2, 'Bob', 35, 'bob@example.com')



```python

```


```python

```


---
**Score: 20**
