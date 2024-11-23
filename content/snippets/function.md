---
title: Function
date: 2024-11-23
author: Your Name
cell_count: 2
score: 0
---

```python
linkedin_found = False

def function(Var1, Var2): 
    if Var2 == 0 and Var1 > 0:
        print("Result One")
    elif Var2 == 1 and Var1 > 0:
        print("Result Two")
    elif Var1 < 1:
        print("Result Three")
    return Var1 - 1

def add(): 
    if True:
        global linkedin_found
        linkedin_found = True        
        
def subtract(): 
    if linkedin_found:
        print("test")
    else:
        print("test1")       


#function(linkedin_found, 1)
add()
subtract()
```

    test



```python

```


---
**Score: 0**
