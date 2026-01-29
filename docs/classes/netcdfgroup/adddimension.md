---
layout: default
title: addDimension
parent: NetCDFGroup
grand_parent: Classes
nav_order: 3
mathjax: true
---

#  addDimension

Add a new coordinate dimension and associated coordinate variable.


---

## Declaration
```matlab
 [dim,var] = addDimension(name,value,options)
```
## Parameters
+ `name`  (char|string) Dimension name.
+ `value`  (:) Coordinate values. Omit or pass [] to create an empty coordinate variable.
+ `options.isUnlimited`  (logical) Mark the dimension as unlimited. Default false.
+ `options.shouldWriteImmediately`  (logical) Write metadata and data to file immediately when possible. Default true.

## Returns
+ `dim`  (NetCDFDimension) Created dimension.
+ `var`  (NetCDFVariable) Created coordinate variable.

## Discussion

  ```matlab
  ncfile.addDimension('x',0:9);
  ```
 
  which will immediately add the dimension and variable data to
  file, OR you may initialize the dimension and an empty
  variable, e.g.,
 
  ```matlab
  ncfile.addDimension('t',length=10,type='double');
  ```
 
  which may be useful when initializing an unlimited
  dimension. In this case you may also want to specify whether
  or not the variable will be complex valued (it will default
  to assuming the variable will be real valued).
 
                
