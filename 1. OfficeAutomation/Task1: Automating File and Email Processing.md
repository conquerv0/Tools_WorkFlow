# 1 Automating File Processing

## 1.1  File Reading
This notebook segments explores how Python can be used in creating, reading and writing files to the disk. 

### 1.1.1  Basics: File and Its Properties
File have two basic properties: `name` and `filepath`. Path points to the location of the file in the computer, name refers to the name of the file at this location. 
We use the function `os.path.join()` to create a file name string: 

```
import os
os.path.join('Quant', 'doc')
```
