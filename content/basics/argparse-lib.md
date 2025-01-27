---
title: Argparse-Lib
date: 2025-01-27
author: Your Name
cell_count: 7
score: 5
---

```python
#import neccessery libraries
```


```python
import argparse
```


```python
import sys
```


```python
#create a method called main
```


```python
def main():
    
    parser = argparse.ArgumentParser(description='SoundScrape. Scrape an artist from SoundCloud.\n')
    parser.add_argument('artist_url', metavar='U', type=str, nargs='*',
                        help='An artist\'s SoundCloud username or URL')
    parser.add_argument('-n', '--num-tracks', type=int, default=sys.maxsize,
                        help='The number of tracks to download')
    parser.add_argument('-g', '--group', action='store_true',
                        help='Use if downloading tracks from a SoundCloud group')
    
    parser.add_argument('-abc', '--abc', type=int, 
                        help='The number of tracks to download')
    
    args = parser.parse_args()
    
    print('args')
    print(args)

    vargs = vars(args)
    print('vargs')    
    print(vargs)
    print(type(vargs))
```


```python
if __name__ == '__main__':
    main()
```

    usage: ipykernel_launcher.py [-h] [-n NUM_TRACKS] [-g] [-abc ABC] [U ...]
    ipykernel_launcher.py: error: unrecognized arguments: -f



    An exception has occurred, use %tb to see the full traceback.


    SystemExit: 2






---
**Score: 5**
