---
layout: default
title: hasDimensionWithName
parent: NetCDFGroup
grand_parent: Classes
nav_order: 19
mathjax: true
---

#  hasDimensionWithName

Determine whether a dimension exists in this group.


---

## Declaration
```matlab
 tf = hasDimensionWithName(dimName)
```
## Parameters
+ `dimName`  (char|string) Dimension name.

## Returns
+ `tf`  (logical) True if the dimension exists.

## Discussion

  ```matlab
  bool = ncfile.hasDimensionWithName('x');
  ```
 
        
