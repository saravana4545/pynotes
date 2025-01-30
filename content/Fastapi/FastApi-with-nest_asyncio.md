---
title: Fastapi-With-Nest Asyncio
date: 2025-01-30
author: Your Name
cell_count: 17
score: 15
---

```python
# Import required modules
```


```python
from fastapi import FastAPI, HTTPException, Query, Path, Depends
from pydantic import BaseModel
from typing import List, Optional
import nest_asyncio
from uvicorn import Config, Server
```


```python
# Enable nested event loops
```


```python
nest_asyncio.apply()
```


```python
# Initialize FastAPI app
```


```python
app = FastAPI()
```


```python
# Simulated database
```


```python
fake_db = []
```


```python
# Book Model
```


```python
class Book(BaseModel):
    id: int
    title: str
    author: str
    description: Optional[str] = None
    rating: Optional[float] = None
```


```python
# Define routes
```


```python
@app.get("/")
def read_root():
    return {"message": "Welcome to the FastAPI app running in JupyterLab!"}
```


```python
@app.post("/books/")
def add_book(book: Book):
    fake_db.append(book.dict())
    return {"message": f"Book '{book.title}' added successfully!"}
```


```python
# Start Uvicorn server inside Jupyter
```


```python
config = Config(app=app, host="127.0.0.1", port=8000, log_level="info")
server = Server(config)
```


```python
# Run the server
```


```python
server.run()
```


---
**Score: 15**
