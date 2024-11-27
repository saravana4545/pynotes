---
title: Cric Using Matplotlib
date: 2024-11-27
author: Your Name
cell_count: 4
score: 0
---

```python
import matplotlib.pyplot as plt
```


```python
def cric_score():
    players = ["Virat Kohli", "MS Dhoni", "Rohit Sharma"]
    runs = [15000, 10500, 14000]
    
    plt.bar(players, runs)
    plt.title("Cricket Players Runs")
    plt.xlabel("Players")
    plt.ylabel("Runs")
    plt.show()
```


```python
print(cric_score())
```


    
![png](Cric_using_matplotlib_files/Cric_using_matplotlib_2_0.png)
    


    None



```python

```


---
**Score: 0**
