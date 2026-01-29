---
layout: default
title: NetCDFFile
parent: NetCDFFile
grand_parent: Classes
nav_order: 1
mathjax: true
---

#  NetCDFFile

Open an existing NetCDF file or create a new file at path.


---

## Declaration
```matlab
 self = NetCDFFile(path,options)
```
## Parameters
+ `path`  (string) file path
+ `options.shouldOverwriteExisting`  logical scalar — delete existing file at path before creating a new dataset
+ `options.shouldUseClassicNetCDF`  logical scalar — create classic (non-NetCDF4) file format
+ `options.shouldReadOnly`  logical scalar — open existing file in read-only mode

## Returns
+ `self`  NetCDFFile instance

## Discussion

  If a file exists at path, it will be opened for reading
  or read/write (depending on options). If no file exists, the
  a new file will be created.
 
              
