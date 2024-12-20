---
title: Make-Qrcode
date: 2024-12-21
author: Your Name
cell_count: 5
score: 5
---

```python
import qrcode
```


```python
def make_qrcode():
    qr = qrcode.QRCode(
        version=1,
        error_correction=qrcode.constants.ERROR_CORRECT_L,
        box_size=10,
        border=4
    )
    qr.add_data("https://github.com/saravana4545/")
    qr.make(fit=True)
    img = qr.make_image(
        fill_color="black",
        back_color="white"
    )
    img.save("qrcode.png")

    return img
```


```python
  print(make_qrcode())
```

    <qrcode.image.pil.PilImage object at 0x7f603616ad80>



```python
    
```


```python

```


---
**Score: 5**
