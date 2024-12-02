---
title: Openpyxl-Lib
date: 2024-12-02
author: Your Name
cell_count: 12
score: 10
---

```python
#import neccessary libraries
```


```python
from openpyxl import Workbook
```


```python
# Create a workbook and add data
```


```python
workbook    = Workbook()
sheet       = workbook.active
sheet.title = "Sample Sheet"
```


```python
#Append the datas in the work book
```


```python
sheet.append(["Name", "Age", "City"])
sheet.append(["Alice", 25, "New York"])
sheet.append(["Bob", 30, "Los Angeles"])
```


```python
#save the datas in the file
```


```python
workbook.save("sample.xlsx")
```


```python
#Then print it
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
**Score: 10**
