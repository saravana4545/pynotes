---
title: Streamlit-Using-Methods
date: 2025-01-21
author: Your Name
cell_count: 10
score: 10
---

```python
import streamlit as st
import numpy as np
import pandas as pd
```


```python
def text_input_example():
    st.title("Text Input Example")
    user_input = st.text_input("Enter your name")
    if user_input:
        st.write(f"Hello, {user_input}!")
```


```python
def checkbox_example():
    if st.checkbox("Show/Hide Text"):
        st.write("This is a hidden text revealed by the checkbox!")
```


```python
def radio_button_example():
    choice = st.radio("Choose your favorite language:", ("Python", "Java", "C++"))
    if choice:
        st.write(f"You selected: {choice}")
```


```python
def slider_example():   
    age = st.sidebar.slider("Select your age", 0, 100, 25)
    st.write(f"Your age is {age}")
```


```python
def line_chart_example():
    chart_data = pd.DataFrame(np.random.randn(20, 3), columns=['A', 'B', 'C'])
    st.line_chart(chart_data)
```


```python
def selectbox_example():
    option = st.selectbox("Select your favorite fruit:", ["Apple", "Banana", "Cherry"])
    st.write(f"You selected: {option}")
```


```python
# Call all the functions
```


```python
text_input_example()
checkbox_example()
radio_button_example()
slider_example()
line_chart_example()
selectbox_example()
```

    2025-01-08 22:15:50.408 WARNING streamlit.runtime.scriptrunner_utils.script_run_context: Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.523 
      [33m[1mWarning:[0m to view this Streamlit app on a browser, run it with the following
      command:
    
        streamlit run /home/saravanakumar/miniconda3/envs/py12/lib/python3.12/site-packages/ipykernel_launcher.py [ARGUMENTS]
    2025-01-08 22:15:50.524 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.525 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.526 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.527 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.527 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.528 Session state does not function when running a script without `streamlit run`
    2025-01-08 22:15:50.529 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.530 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.531 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.532 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.533 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.534 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.536 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.537 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.538 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.539 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.540 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.541 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.542 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.543 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.544 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.544 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.545 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.546 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.547 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.550 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.551 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.551 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.552 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.552 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.553 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.553 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.887 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.888 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.889 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.889 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.890 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.890 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.891 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.892 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.892 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.893 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.893 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.
    2025-01-08 22:15:50.894 Thread 'MainThread': missing ScriptRunContext! This warning can be ignored when running in bare mode.



```python

```


---
**Score: 10**
