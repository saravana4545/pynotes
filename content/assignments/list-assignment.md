---
title: List-Assignment
date: 2025-01-30
author: Your Name
cell_count: 9
score: 5
---

```python
# Input 5 integers
numbers = []
```


```python
for i in range(5):
    num = int(input(f"Enter number {i + 1}: "))
    numbers.append(num)
```

    Enter number 1:  45
    Enter number 2:  24
    Enter number 3:  52
    Enter number 4:  42
    Enter number 5:  10



```python
# Calculate sum and average
```


```python
total_sum = sum(numbers)
average = total_sum / len(numbers)
```


```python
# Display results
```


```python
print("\nNumbers entered:", numbers)
```

    
    Numbers entered: [45, 24, 52, 42, 10]



```python
print("Sum:", total_sum)
```

    Sum: 173



```python
print("Average:", average)
```

    Average: 34.6



```python

```


---
**Score: 5**
