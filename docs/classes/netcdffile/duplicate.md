---
layout: default
title: duplicate
parent: NetCDFFile
grand_parent: Classes
nav_order: 4
mathjax: true
---

#  duplicate

the NetCDF dataset to a new file.


---

## Declaration
```matlab
 ncfile = duplicate(path,options)
```
## Parameters
+ `path`  any — destination file path
+ `options.shouldOverwriteExisting`  logical scalar (1x1) — overwrite destination if it exists
+ `options.indexRange`  dictionary (string -> cell) — per-variable slicing ranges forwarded to addDuplicateGroup

## Returns
+ `ncfile`  NetCDFFile instance — duplicated dataset handle

## Discussion

  Creates a new NetCDFFile at the requested path and copies the
  current group hierarchy, dimensions, variables, and attributes
  using addDuplicateGroup. Optionally restricts copied data via
  indexRange.
 
            
