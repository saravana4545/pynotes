---
title: Fastapi-Basic
date: 2024-11-29
author: Your Name
cell_count: 8
score: 5
---

```python
from fastapi import FastAPI
```


```python
import nest_asyncio
```


```python
from uvicorn import Config, Server
```


```python
nest_asyncio.apply()
```


```python
app = FastAPI()
```


```python
@app.get("/")
def read_root():
    return {"message": "Hello from FastAPI in JupyterLab!"}


# Run FastAPI server
config = Config(
    app      =app,
    host     ="127.0.0.1",
    port     =8000,
    log_level="info"
)

server = Server(config)

server.run()
```


```python

```


```python

```


---
**Score: 5**
