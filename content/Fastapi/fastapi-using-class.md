---
title: Fastapi-Using-Class
date: 2025-01-25
author: Your Name
cell_count: 15
score: 15
---

```python
#import neccessary libraries
```


```python
from fastapi import FastAPI, HTTPException
from pydantic import BaseModel
from typing import List
```


```python
app = FastAPI()
```


```python
# Pydantic model for book data
```


```python
class Book(BaseModel):
    id    : int
    title : str
    author: str
```


```python
# BookStore class to manage books
```


```python
class BookStore:
    def __init__(self):
        self.books = []  # Start with an empty list

    def get_all_books(self):
        return self.books

    def get_book_by_id(self, book_id: int):
        for book in self.books:
            if book.id == book_id:
                return book
        return None

    def add_book(self, book: Book):
        if any(b.id == book.id for b in self.books):
            raise HTTPException(status_code=400, detail="Book with this ID already exists")
        self.books.append(book)
        return book

```


```python
# Create an instance of the class
```


```python
book_store = BookStore()
```


```python
# GET method to fetch all books
```


```python
@app.get("/books/", response_model=List[Book])
async def get_books():
    return book_store.get_all_books()
```


```python
# GET method to fetch a book by ID
```


```python
@app.get("/books/{book_id}", response_model=Book)
async def get_book(book_id: int):
    book = book_store.get_book_by_id(book_id)
    if not book:
        raise HTTPException(status_code=404, detail="Book not found")
    return book
```


```python
# POST method to add a new book
```


```python
@app.post("/books/", response_model=Book)
async def add_book(book: Book):
    return book_store.add_book(book)
```


---
**Score: 15**
