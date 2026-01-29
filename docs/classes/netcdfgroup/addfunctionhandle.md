---
layout: default
title: addFunctionHandle
parent: NetCDFGroup
grand_parent: Classes
nav_order: 5
mathjax: true
---

#  addFunctionHandle

Add a lazily-evaluated variable backed by a function handle.


---

## Declaration
```matlab
 var = addFunctionHandle(name,value,options)
```
## Parameters
+ `name`  (char|string) Variable name.
+ `value`  (function_handle) Function handle used to generate variable data on demand.
+ `options.dimNames`  (cell|string) Dimension names defining the variable.
+ `options.isComplex`  (logical) Create a complex variable wrapper. Default false.

## Returns
+ `var`  (NetCDFVariable) Created variable object.

## Discussion

  ```matlab
  m = 1; b = 2;
  f = @(x) m*x + b;
  ncfile.addFunctionHandle('f',f);
  ```
 
              
