---
title: Class-Assignment
date: 2025-03-27
author: Your Name
cell_count: 6
score: 5
---

```python
# Created at 27-03-2025
```


```python
class Parent1:
    def __init__(self, a, b, c):
        self.a = a
        self.b = b
        self.c = c

    def add(self, a, b, c):
        a1 = self.a + self.b
        a2 = self.b + self.c
        print(f"{a} and {b} is {a1}")
        print(f"{b} and {c} is {a2}")
        pass
        return a1, a2

    def sub(self, a, b):
        s1 = a - b
        s2 = self.add(a,b,c)
        print(f"{a} and {b} is {s1}")
        print(f"a1 and a2 is {s2}")
        return s1, s2
```


```python
class Parent2(Parent1):
    def multi(self, s1, s2, a1, a2):
        m1 = super().sub(s1 * s2)
        m2 = super().add(a1 * a2)
        print(f"s1 and s2 is {m1}")
        print(f"a1 and a2 is {m2}")
        pass
        return m1, m2

    def div(self, m1, m2):
        d1 = m1 / m2
        print(f"m1 by m2 is {d1}")
        pass
        return d1
```


```python
class Child(Parent2):
    def calculate(self, m1, m2):
        answer = self.div(m1, m2)
        return answer

final_result = Child(a=2,b=3,c=6)
final_result.sub(2,3)
print(f"Final Answer:{final_result}")
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    Cell In[6], line 7
          4         return answer
          6 final_result = Child(a=2,b=3,c=6)
    ----> 7 final_result.sub(2,3)
          8 print(f"Final Answer:{final_result}")


    Cell In[2], line 17, in Parent1.sub(self, a, b)
         15 def sub(self, a, b):
         16     s1 = a - b
    ---> 17     s2 = self.add(a,b,c)
         18     print(f"{a} and {b} is {s1}")
         19     print(f"a1 and a2 is {s2}")


    NameError: name 'c' is not defined



```python
# Example Usage

```


```python

```


---
**Score: 5**
