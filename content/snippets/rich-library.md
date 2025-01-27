---
title: Rich-Library
date: 2025-01-27
author: Your Name
cell_count: 6
score: 5
---

```python
from rich.console import Console
```


```python
from rich.table import Table
```


```python
console = Console()
```


```python
def create_table():
    table = Table(title="Programming Languages")
    table.add_column("Language", style="bold cyan")
    table.add_column("Creator", style="green")
    table.add_column("Year", justify="right")

    table.add_row("Python", "Guido van Rossum", "1991")
    table.add_row("JavaScript", "Brendan Eich", "1995")
    table.add_row("Go", "Robert Griesemer", "2009")

    console.print(table)
```


```python
print(create_table())
```


<pre style="white-space:pre;overflow-x:auto;line-height:normal;font-family:Menlo,'DejaVu Sans Mono',consolas,'Courier New',monospace"><span style="font-style: italic">         Programming Languages          </span>
┏━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━┳━━━━━━┓
┃<span style="font-weight: bold"> Language   </span>┃<span style="font-weight: bold"> Creator          </span>┃<span style="font-weight: bold"> Year </span>┃
┡━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━╇━━━━━━┩
│<span style="color: #008080; text-decoration-color: #008080; font-weight: bold"> Python     </span>│<span style="color: #008000; text-decoration-color: #008000"> Guido van Rossum </span>│ 1991 │
│<span style="color: #008080; text-decoration-color: #008080; font-weight: bold"> JavaScript </span>│<span style="color: #008000; text-decoration-color: #008000"> Brendan Eich     </span>│ 1995 │
│<span style="color: #008080; text-decoration-color: #008080; font-weight: bold"> Go         </span>│<span style="color: #008000; text-decoration-color: #008000"> Robert Griesemer </span>│ 2009 │
└────────────┴──────────────────┴──────┘
</pre>



    None



```python

```


---
**Score: 5**
