---
title: Squarify-Lib
date: 2025-03-27
author: Your Name
cell_count: 14
score: 10
---

```python
#import neccessery libraries
```


```python
import squarify
```


```python
# these values define the coordinate system for the returned rectangles
# the values will range from x to x + width and y to y + height
```


```python
x = 0.
y = 0.
width  = 700.
height = 433.

values = [500, 433, 78, 25, 25, 7]
```


```python
# values must be sorted descending (and positive, obviously)
```


```python
values.sort(reverse=True)
```


```python
# the sum of the values must equal the total area to be laid out
```


```python
values = squarify.normalize_sizes(values, width, height)
```


```python
# returns a list of rectangles
```


```python
rects = squarify.squarify(values, x, y, width, height)
```


```python
# padded rectangles will probably visualize better for certain cases
```


```python
padded_rects = squarify.padded_squarify(values, x, y, width, height)
```


```python
print(padded_rects)
```

    [{'x': 1.0, 'y': 1.0, 'dx': 325.7153558052434, 'dy': 431.0}, {'x': 328.7153558052434, 'y': 1.0, 'dx': 370.2846441947566, 'dy': 328.0862676056338}, {'x': 328.7153558052434, 'y': 331.0862676056338, 'dx': 213.0977944236371, 'dy': 100.9137323943662}, {'x': 543.8131502288805, 'y': 331.0862676056338, 'dx': 66.94160077680677, 'dy': 100.9137323943662}, {'x': 612.7547510056874, 'y': 331.0862676056338, 'dx': 86.24524899431273, 'dy': 78.40135343309854}, {'x': 612.7547510056874, 'y': 411.4876210387323, 'dx': 86.2452489943124, 'dy': 20.51237896126767}]



```python

```


---
**Score: 10**
