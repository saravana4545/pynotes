---
title: Html-Lib
date: 2024-12-02
author: Your Name
cell_count: 5
score: 5
---

```python
import html
```


```python
def convert_text(text):
    output_text = html.unescape(text)
    return output_text
```


```python
def startpy():
    text       = "&lt;ul&gt;&lt;li&gt;one.&lt;/li&gt;&lt;li&gt;two.&lt;/li&gt;&lt;/ul&gt;"
    final_html = convert_text(text)
    print(f'original_string :{text}\nfinal_html:{final_html}')
```


```python
if __name__ == '__main__':
    startpy()
```

    original_string :&lt;ul&gt;&lt;li&gt;one.&lt;/li&gt;&lt;li&gt;two.&lt;/li&gt;&lt;/ul&gt;
    final_html:<ul><li>one.</li><li>two.</li></ul>



```python

```


---
**Score: 5**
