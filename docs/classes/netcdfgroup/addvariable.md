---
layout: default
title: addVariable
parent: NetCDFGroup
grand_parent: Classes
nav_order: 7
mathjax: true
---

#  addVariable

Add a real or complex variable to the group.


---

## Declaration
```matlab
 var = addVariable(name,dimNames,value,options)
```
## Parameters
+ `name`  (char|string) Variable name.
+ `dimNames`  (cell|string) Dimension names (coordinate dimensions) defining the variable.
+ `value`  (:) Variable data. Omit or pass [] to create metadata without writing data.
+ `options.isComplex`  (logical) Create a complex variable wrapper. Default false.
+ `options.shouldWriteImmediately`  (logical) Write metadata and data to file immediately when possible. Default true.

## Returns
+ `var`  (NetCDFVariable) Created variable object.

## Discussion

  ```matlab
  ncfile.addVariable('fluid-tracer', {'x','y','t'}, myVariableData);
  ```
 
  or intializes an variable without setting the data,
  ```matlab
  ncfile.addVariable('fluid-tracer', {'x','y','t'});
  ```
 
                
