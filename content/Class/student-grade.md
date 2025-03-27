---
title: Student-Grade
date: 2025-03-27
author: Your Name
cell_count: 5
score: 5
---

```python
# Created at 27-03-2025
```


```python
class Student:
    def __init__(self, name, marks):
        self.name = name
        self.marks = marks

    def grade(self):
        if self.marks >= 90:
            return "A"
        elif self.marks >= 80:
            return "B"
        elif self.marks >= 70:
            return "C"
        elif self.marks >= 60:
            return "D"
        else:
            return "F"
```


```python
# Create a student object
```


```python
student = Student("John", 85)
print(f"{student.name} scored {student.marks} and got grade {student.grade()}")
```

    John scored 85 and got grade B



```python

```


---
**Score: 5**
