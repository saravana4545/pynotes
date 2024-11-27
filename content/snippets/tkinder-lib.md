---
title: Tkinder-Lib
date: 2024-11-27
author: Your Name
cell_count: 7
score: 5
---

```python
import tkinter as tk
```


```python
def greet():
    label.config(
        text=f"Hello,{entry.get()}!"
    )
```


```python
# Create GUI
root = tk.Tk()
root.title("Simple GUI")
```




    ''




```python
label = tk.Label(
    root,
    text="Enter your name:"
)
label.pack()
```


```python
entry = tk.Entry(root)
entry.pack()
```


```python
button = tk.Button(
    root,
    text="Greet",
    command=greet
)
button.pack()

root.mainloop()
```


```python

```


---
**Score: 5**
