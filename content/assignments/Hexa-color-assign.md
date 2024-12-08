---
title: Hexa-Color-Assign
date: 2024-12-08
author: Your Name
cell_count: 16
score: 15
---

```python
#import neccesary libraries
```


```python
import os
from flask import Flask, render_template, request
from pymongo import MongoClient
from dotenv import load_dotenv
import webcolors
```


```python
# Load environment variables
```


```python
load_dotenv()
```




    False




```python
# Initialize Flask app
```


```python
app = Flask(__name__)
```


```python

```


```python
# Connect to MongoDB
```


```python
client     = MongoClient(os.environ["MONGO_URL"])
db         = client['DB_NAME']
collection = db['DB_COLLECTION']
```


```python

```


```python
#create a method and route for get the color name and it's hexadecimal_code
```


```python
@app.route('/', methods=['POST', 'GET'])
def home():
    if request.method == "POST":
        colour_name = request.values.get('colour_name')
        
        # Check if the color name is valid
        try:
            hex_value = webcolors.name_to_hex(colour_name)

        except ValueError:
            return render_template(
                'index.html',
                error=f"'{colour_name}' is not a name of color."
            )

        # Check if the color already exists in the database
        existing_color = collection.find_one({"colour_name": colour_name.lower()})
        if existing_color:
            return render_template(
                'index.html',
                color=existing_color
            )

        # Add new color to the database
        color = {
            'colour_name': colour_name.lower(),
            'Hexa_code': hex_value
        }
        collection.insert_one(color)
        return render_template('index.html', color=color)

    return render_template('index.html')
```


```python
#This line checks if the script is being run directly or imported
```


```python
if __name__ == '__main__':
    app.run(
        debug = True,
        port  = 4545
    )
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    Cell In[3], line 2
          1 if __name__ == '__main__':
    ----> 2     app.run(
          3         debug = True,
          4         port  = 4545
          5     )


    NameError: name 'app' is not defined



```python

```


```python

```


---
**Score: 15**
