---
title: Dash-Framework
date: 2024-11-22
author: Your Name
cell_count: 5
score: 5
---

```python
from dash import Dash, html
```


```python
app = Dash(__name__)
```


```python
def dash_frame():
    app.layout = html.Div([
        html.H1("Hello Dash!"),
        html.P("This is a simple dashboard.")
    ])
    return app
```


```python
if __name__ == "__main__":
    app.run_server(debug=True)
```



<iframe
    width="100%"
    height="650"
    src="http://127.0.0.1:8050/"
    frameborder="0"
    allowfullscreen

></iframe>




```python

```


---
**Score: 5**