---
title: Colorama-Lib
date: 2024-12-04
author: Your Name
cell_count: 7
score: 5
---

```python
#import colorama
```


```python
from colorama import Fore, Back, Style
```


```python
#create a method called colorful_message
```


```python
def colorful_message(text, foreground, background=None, style=None):
    formatted_text = ""
    if foreground:
        formatted_text += foreground
    if background:
        formatted_text += background
    if style:
        formatted_text += style
    formatted_text += text + Style.RESET_ALL
    print(formatted_text)
```


```python
# Example usage
```


```python
colorful_message(
    "Warning!",
    Fore.BLACK,
    Back.RED,
    Style.BRIGHT
)
colorful_message(
    "Info",
    Fore.CYAN
)
colorful_message(
    "Success!",
    Fore.GREEN,
    Style.BRIGHT
)
```

    [30m[41m[1mWarning![0m
    [36mInfo[0m
    [32m[1mSuccess![0m



```python

```


---
**Score: 5**
