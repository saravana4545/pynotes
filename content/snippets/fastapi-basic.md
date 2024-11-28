---
title: Fastapi-Basic
date: 2024-11-28
author: Your Name
cell_count: 8
score: 5
---

```python
from fastapi import FastAPI
```


```python
from fastapi.responses import HTMLResponse
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
@app.get("/", response_class=HTMLResponse)
def read_root():
    return "<h1>Welcome to FastAPI in JupyterLab!</h1>"

# Run the server
config = Config(
    app      =app,
    host     ="127.0.0.1",
    port     =8000,
    log_level="info"
)
server = Server(config)
server.run()
```

    INFO:     Started server process [11011]
    INFO:     Waiting for application startup.
    INFO:     Application startup complete.
    INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)


    INFO:     127.0.0.1:46628 - "GET /doc HTTP/1.1" 404 Not Found
    INFO:     127.0.0.1:46628 - "GET /favicon.ico HTTP/1.1" 404 Not Found
    INFO:     127.0.0.1:39180 - "GET /docs HTTP/1.1" 200 OK
    INFO:     127.0.0.1:43084 - "GET /openapi.json HTTP/1.1" 200 OK
    INFO:     127.0.0.1:43094 - "GET / HTTP/1.1" 200 OK



```python

```


---
**Score: 5**
