---
title: Yaml-Lib
date: 2024-11-23
author: Your Name
cell_count: 3
score: 0
---

```python
import yaml
```


```python
# Read YAML
yaml_data = """
name: Alice
age: 25
skills:
  - Python
  - Machine Learning
"""
data = yaml.safe_load(yaml_data)
print(data)

# Write YAML
with open("output.yaml", "w") as file:
    yaml.dump(data, file)

```

    {'name': 'Alice', 'age': 25, 'skills': ['Python', 'Machine Learning']}



```python

```


---
**Score: 0**
