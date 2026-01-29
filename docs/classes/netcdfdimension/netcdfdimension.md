---
layout: default
title: NetCDFDimension
parent: NetCDFDimension
grand_parent: Classes
nav_order: 1
mathjax: true
---

#  NetCDFDimension

create a NetCDFDimension


---

## Declaration
```matlab
 self = NetCDFDimension(group,options)
```
## Parameters
+ `group`  a NetCDFGroup instance
+ `name (optional)`  name of the dimension (string)
+ `nPoints (optional)`  0 or more, inf if unlimited
+ `id (optional)`  id of an existing dimension

## Returns
+ `self`  a NetCDFDimension object

## Discussion

  All dimensions must have a group to which they belong. If you
  initialize by passing an id, then the dimension will be
  intialized from file. If you initialize by passing the name
  and the number of points, then a new dimension will be
  created and added to file.
 
              
