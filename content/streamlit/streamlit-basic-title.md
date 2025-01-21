---
title: Streamlit-Basic-Title
date: 2025-01-21
author: Your Name
cell_count: 14
score: 10
---

```python
import streamlit as st
import pandas as pd
import numpy as np
```


```python
# To create Title of the app
```


```python
st.title("Simple Streamlit App")
```

    2025-01-08 20:43:57.370 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 20:43:57.372 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.





    DeltaGenerator()




```python
# To create Adding a markdown
```


```python
st.markdown("### Welcome to this Streamlit POC!")
```

    2025-01-08 20:43:58.192 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 20:43:58.194 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.





    DeltaGenerator()




```python
# Displaying some data
```


```python
st.write("Here's a random dataset:")
```

    2025-01-08 20:43:58.818 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 20:43:58.820 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 20:43:58.821 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 20:43:58.822 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.



```python
# Generating a random dataframe
```


```python
data = pd.DataFrame(
    np.random.randn(10, 5),
    columns=('col %d' % i for i in range(5))
)

st.write(data)
```

    2025-01-08 20:43:59.359 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 20:43:59.360 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.



```python
# Adding a button widget
```


```python
if st.button("Generate new data"):
    data = pd.DataFrame(
        np.random.randn(10, 5),
        columns=('col %d' % i for i in range(5))
    )
    st.write(data)
```

    2025-01-08 20:44:00.050 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 20:44:00.051 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 20:44:00.052 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 20:44:00.054 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 20:44:00.054 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.



```python
# Adding a slider widget
```


```python
st.write("Select a number with the slider:")
number = st.slider("Pick a number", 0, 100, 50)

st.write(f"The number you selected is {number}")
```

    2025-01-08 20:44:00.963 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 20:44:00.965 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 20:44:00.966 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 20:44:00.967 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 20:44:00.968 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 20:44:00.968 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 20:44:00.969 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 20:44:00.970 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 20:44:00.970 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 20:44:00.971 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 20:44:00.972 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 20:44:00.973 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 20:44:00.973 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.



```python

```


---
**Score: 10**
