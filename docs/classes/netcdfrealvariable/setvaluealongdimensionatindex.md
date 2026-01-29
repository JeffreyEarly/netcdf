---
layout: default
title: setValueAlongDimensionAtIndex
parent: NetCDFRealVariable
grand_parent: Classes
nav_order: 6
mathjax: true
---

#  setValueAlongDimensionAtIndex

append new data to an existing variable


---

## Declaration
```matlab
 setValueAlongDimensionAtIndex(data,dimension,index)
```
## Parameters
+ `data`  variable data
+ `dimension`  the variable dimension along which to concatenate
+ `index`  index at which to write data

## Discussion

  concatenates data along a variable dimension (such as a time
  dimension).
 
  ```matlab
  variable.setValueAlongDimensionAtIndex(data,dimensionName,index);
  ```
 
          
