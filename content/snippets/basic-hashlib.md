---
title: Basic-Hashlib
date: 2025-01-08
author: Your Name
cell_count: 11
score: 10
---

```python
#import hashlib module
```


```python
import hashlib
```


```python
# Input string
```


```python
data = "Hello, World!"
```


```python
# Generate MD5 hash
```


```python
md5_hash = hashlib.md5(data.encode()).hexdigest()
print("MD5 Hash:", md5_hash)
```

    MD5 Hash: 65a8e27d8879283831b664bd8b7f0ad4



```python
# Generate SHA-1 hash
```


```python
sha1_hash = hashlib.sha1(data.encode()).hexdigest()
print("SHA-1 Hash:", sha1_hash)
```

    SHA-1 Hash: 0a0a9f2a6772942557ab5355d76af442f8f65e01



```python
# Generate SHA-256 hash
```


```python
sha256_hash = hashlib.sha256(data.encode()).hexdigest()
print("SHA-256 Hash:", sha256_hash)
```

    SHA-256 Hash: dffd6021bb2bd5b0af676290809ec3a53191dd81c7f70a4b28688a362182986f



```python

```


---
**Score: 10**
