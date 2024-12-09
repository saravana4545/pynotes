---
title: Cricket-Score
date: 2024-12-09
author: Your Name
cell_count: 9
score: 5
---

```python
#import neccessory libraries
```


```python
import time
from random import randint
```


```python
#create a method called get_ball_in_words()
```


```python
def get_ball_in_words(ball):
    if(ball == 1):
        return 'first'
    elif(ball == 2):
        return 'second'
    elif(ball == 3):
        return 'third'
    elif(ball == 4):
        return 'fourth'
    elif(ball == 5):
        return 'fifth'
    elif(ball == 6):
        return 'last' 
```


```python
#create a method and set the loop func
```


```python
def play_over(bowler, batsman):
    
    for i in range(6):       
        ball = i + 1
             
        time.sleep(randint(1, 4))
        print(bowler+' bowling '+get_ball_in_words(ball)+' ball : ')
        
        run  = randint(0, 6)
        print(batsman+' hits '+str(run))
```


```python
#call the method and put the value for perameter
```


```python
play_over('STARC','ROHIT')
```

    STARC bowling first ball : 
    ROHIT hits 1
    STARC bowling second ball : 
    ROHIT hits 3
    STARC bowling third ball : 
    ROHIT hits 4
    STARC bowling fourth ball : 
    ROHIT hits 3
    STARC bowling fifth ball : 
    ROHIT hits 2
    STARC bowling last ball : 
    ROHIT hits 6



```python

```


---
**Score: 5**
