---
title: Base64-Lib
date: 2024-11-23
author: Your Name
cell_count: 4
score: 0
---

```python
import base64
```


```python
def encode_data(userid, email, expiry_date):
    data = f"{userid}|{email}|{expiry_date}"
    encoded_data = base64.urlsafe_b64encode(data.encode()).decode()
    return encoded_data

def decode_data(encoded_data):
    decoded_data = base64.urlsafe_b64decode(encoded_data.encode()).decode()
    userid, email, expiry_date = decoded_data.split('|')
    return userid, email, expiry_date

def startpy():

    # Example Usage
    encoded_value = encode_data('123', 'saravana4545@gmail.com', '2024-12-31')
    print(f"Encoded: {encoded_value}")
    # Example Usage
    decoded_value = decode_data(encoded_value)
    print(f"Decoded: {decoded_value}")
    pass
```


```python
if __name__ == '__main__':
    startpy()
```

    Encoded: MTIzfHNhcmF2YW5hNDU0NUBnbWFpbC5jb218MjAyNC0xMi0zMQ==
    Decoded: ('123', 'saravana4545@gmail.com', '2024-12-31')



```python

```


---
**Score: 0**