---
title: Openpyxl-Lib
date: 2024-11-29
author: Your Name
cell_count: 7
score: 5
---

```python
from openpyxl import Workbook
```


```python
# Create a workbook and add data
workbook    = Workbook()
sheet       = workbook.active
sheet.title = "Sample Sheet"
```


```python
sheet.append(["Name", "Age", "City"])
sheet.append(["Alice", 25, "New York"])
sheet.append(["Bob", 30, "Los Angeles"])
```


```python
workbook.save("sample.xlsx")
```


```python
print("Excel file created!")
```

    Excel file created!



```python

```


```python

```


---
**Score: 5**
