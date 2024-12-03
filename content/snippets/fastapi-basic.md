---
title: Fastapi-Basic
date: 2024-12-03
author: Your Name
cell_count: 12
score: 10
---

```python
#import all neccessary libraries
```


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
#connect the FastAPI
```


```python
app = FastAPI()
```


```python
#create a route for get method
```


```python
@app.get("/")
def read_root():
    return {"message": "Hello from FastAPI in JupyterLab!"}
```


```python
# Run FastAPI server
```


```python
config = Config(
    app      =app,
    host     ="127.0.0.1",
    port     =8000,
    log_level="info"
)

server = Server(config)

server.run()
```

    INFO:     Started server process [3939]
    INFO:     Waiting for application startup.
    INFO:     Application startup complete.
    INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)



```python

```


---
**Score: 10**
