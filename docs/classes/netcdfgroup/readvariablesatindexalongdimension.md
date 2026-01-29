---
layout: default
title: readVariablesAtIndexAlongDimension
parent: NetCDFGroup
grand_parent: Classes
nav_order: 26
mathjax: true
---

#  readVariablesAtIndexAlongDimension

Read variables at a single index along a named dimension.


---

## Declaration
```matlab
 varargout = readVariablesAtIndexAlongDimension(dimName,index,variableNames)
```
## Parameters
+ `dimName`  (char|string) Dimension name to index.
+ `index`  (double) 1-based index along dimName.
+ `variableNames`  (cell|string) Variable names or paths to read.

## Returns
+ `varargout`  (cell) Variable data slices returned in the same order as variableNames.

## Discussion

  ```matlab
  [u,v] = ncfile.readVariablesAtIndexAlongDimension('t',100,'u','v');
  ```
 
            
