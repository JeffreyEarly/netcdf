---
layout: default
title: readVariables
parent: NetCDFGroup
grand_parent: Classes
nav_order: 25
mathjax: true
---

#  readVariables

Read one or more variables from file.


---

## Declaration
```matlab
 varargout = readVariables(variableNames)
```
## Parameters
+ `variableNames`  (cell|string) Variable names or paths to read.

## Returns
+ `varargout`  (cell) Variable data returned in the same order as variableNames.

## Discussion

  ```matlab
  [x,y] = ncfile.readVariables('x','y');
  ```
 
        
