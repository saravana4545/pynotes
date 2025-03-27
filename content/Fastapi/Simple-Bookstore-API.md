---
title: Simple-Bookstore-Api
date: 2025-03-27
author: Your Name
cell_count: 33
score: 30
---

```python
#import neccesary libraries
```


```python
from fastapi import FastAPI, HTTPException, Query, Path, Depends
from pydantic import BaseModel
from typing import List, Optional
```


```python

```


```python
app = FastAPI()
```


```python

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
# Dependency: Simulating a database check
```


```python
def get_db():
    if not fake_db:
        raise HTTPException(status_code=404, detail="No books found")
    return fake_db
```


```python
# Route to list all books
```


```python

```


```python
@app.get("/books/", response_model=List[Book])
def list_books(db=Depends(get_db)):
    return db
```


```python
# Route to get a specific book by ID
```


```python

```


```python
@app.get("/books/{book_id}", response_model=Book)
def get_book(book_id: int = Path(..., description="ID of the book to retrieve")):
    for book in fake_db:
        if book["id"] == book_id:
            return book
    raise HTTPException(status_code=404, detail="Book not found")
```


```python
# Route to search books by title or author
```


```python

```


```python
@app.get("/books/search/", response_model=List[Book])
def search_books(
    title: Optional[str]  = Query(None, description="Search by book title"),
    author: Optional[str] = Query(None, description="Search by author name"),
    db=Depends(get_db),
):
    results = [book for book in db if (title and title.lower() in book["title"].lower()) or
               (author and author.lower() in book["author"].lower())]
    if not results:
        raise HTTPException(status_code=404, detail="No matching books found")
    return results
```


```python
# Route to add a new book
```


```python

```


```python
@app.post("/books/", response_model=Book, status_code=201)
def add_book(book: Book):
    # Check if book ID already exists
    if any(existing_book["id"] == book.id for existing_book in fake_db):
        raise HTTPException(status_code=400, detail="Book with this ID already exists")
    fake_db.append(book.dict())
    return book
```


```python
# Route to update a book
```


```python

```


```python
@app.put("/books/{book_id}", response_model=Book)
def update_book(book_id: int, updated_book: Book):
    for idx, book in enumerate(fake_db):
        if book["id"] == book_id:
            fake_db[idx] = updated_book.dict()
            return updated_book
    raise HTTPException(status_code=404, detail="Book not found")
```


```python
# Route to delete a book
```


```python

```


```python
@app.delete("/books/{book_id}", status_code=204)
def delete_book(book_id: int):
    for book in fake_db:
        if book["id"] == book_id:
            fake_db.remove(book)
            return
    raise HTTPException(status_code=404, detail="Book not found")
```


```python
# Sample Data Loader Route
```


```python

```


```python
@app.post("/books/load_sample/")
def load_sample_books():
    sample_books = [
        {"id": 1, "title": "1984", "author": "George Orwell", "description": "Dystopian novel", "rating": 4.8},
        {"id": 2, "title": "To Kill a Mockingbird", "author": "Harper Lee", "description": "Classic novel", "rating": 4.9},
        {"id": 3, "title": "The Great Gatsby", "author": "F. Scott Fitzgerald", "description": "1920s novel", "rating": 4.7}
    ]
    fake_db.extend(sample_books)
    return {"message": "Sample books loaded successfully!"}
```


```python

```


```python

```


---
**Score: 30**
