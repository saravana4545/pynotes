---
title: Employee-Details
date: 2025-01-08
author: Your Name
cell_count: 6
score: 5
---

```python
class Employee:
    def __init__(self, emp_id, name, salary):
        self.emp_id = emp_id
        self.name = name
        self.salary = salary

    def display_details(self):
        print(f"ID: {self.emp_id}, Name: {self.name}, Salary: {self.salary}")
```


```python
# List of employees
```


```python
employees = [
    Employee(1, "Alice", 50000),
    Employee(2, "Bob", 60000),
    Employee(3, "Charlie", 70000),
]
```


```python
# Display details of each employee
```


```python
for emp in employees:
    emp.display_details()
```

    ID: 1, Name: Alice, Salary: 50000
    ID: 2, Name: Bob, Salary: 60000
    ID: 3, Name: Charlie, Salary: 70000



```python

```


---
**Score: 5**
