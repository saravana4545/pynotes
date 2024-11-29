---
title: H5Py-Lib
date: 2024-11-29
author: Your Name
cell_count: 4
score: 0
---

```python
import h5py
```


```python
def startpy():
    file    = h5py.File('dset.h5','w')
    dataset = file.create_dataset(
        "dset",
        (4, 6),
        h5py.h5t.STD_I32BE
    )
    print("Dataset dataspace is", dataset.shape)
    print("Dataset Numpy datatype is", dataset.dtype)
    print("Dataset name is", dataset.name)
    print("Dataset is a member of the group", dataset.parent)
    print("Dataset was created in the file", dataset.file)

    file.close()
```


```python
if __name__ == '__main__':
    startpy()
```

    Dataset dataspace is (4, 6)
    Dataset Numpy datatype is >i4
    Dataset name is /dset
    Dataset is a member of the group <HDF5 group "/" (1 members)>
    Dataset was created in the file <HDF5 file "dset.h5" (mode r+)>



```python

```


---
**Score: 0**
