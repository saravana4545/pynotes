---
title: Multipication
date: 2025-01-21
author: Your Name
cell_count: 5
score: 5
---

```python
class Calculate:

    def __init__(self, num1, num2, num3):
        self.num1 = num1
        self.num2 = num2
        self.num3 = num3

    def multyply(self,num1, num2):
        mult = num1 * num2
        print(f"multy:{mult}")
        return mult
    
    def multyply_2(self, num2, num3):
        mult_2 = num2 * num3
        print(f"multply second num: {mult_2}")
        return mult_2
```


```python
class Calculate_2(Calculate):
    def __init__(self, num1, num2, num3):
        super().__init__(num1, num2, num3)
    
    def add(self, num1 , num2):
        return num1 + num2
    
    def add_first_values(self):
        results  = super().multyply(self.num1, self.num2)
        result_2 = super().multyply_2(self.num2, self.num3)
        
        mult = self.add(results, result_2)
        print(f"result :{mult}")
```


```python
result = Calculate_2(num1=2, num2=3,num3=5)
```


```python
result.multyply(num1=1, num2=2)
```

    multy:2





    2




```python

```


---
**Score: 5**
