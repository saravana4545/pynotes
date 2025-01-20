---
title: Cric Using Matplotlib
date: 2025-01-20
author: Your Name
cell_count: 7
score: 5
---

```python
#import neccessary libraries
```


```python
import matplotlib.pyplot as plt
```


```python
#create a method called cric_score
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
#print the method
```


```python
print(cric_score())
```


    
![png](Cric_using_matplotlib_files/Cric_using_matplotlib_5_0.png)
    


    None



```python

```


---
**Score: 5**
