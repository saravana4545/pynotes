---
title: Pdf-Creator
date: 2025-01-21
author: Your Name
cell_count: 5
score: 5
---

```python
from fpdf  import FPDF
```


```python
p = FPDF()
```


```python
p.add_page()
p.set_font("Arial", size=12)
p.cell(200,10,txt='USER INFORMATION', ln=True, align='c')

p.ln(10)
p.cell(200, 10, txt="Address:", ln=True)
p.cell(200, 10, txt="1234 Main Street", ln=True)
p.cell(200, 10, txt="Apt. 101", ln=True)
p.cell(200, 10, txt="perth,optus stadium, australia", ln=True)

p.ln(20)
```


```python
for i in range(2,6):
    p.add_page()
    p.cell(200,10, txt=f'This is page {i}.',ln=True)

p.output('example.pdf')
print("pdf created")
```

    pdf created



```python

```


---
**Score: 5**
