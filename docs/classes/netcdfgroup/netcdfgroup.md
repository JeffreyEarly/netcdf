---
layout: default
title: NetCDFGroup
parent: NetCDFGroup
grand_parent: Classes
nav_order: 1
mathjax: true
---

#  NetCDFGroup

Create and manage a NetCDF group.


---

## Declaration
```matlab
 grp = NetCDFGroup(options)
```
## Parameters
+ `options.name`  (char) Group name.
+ `options.id`  (double) NetCDF group ID to load from an existing file.
+ `options.parentGroup`  (NetCDFGroup) Parent group. Use [] for the root group.

## Returns
+ `grp`  (NetCDFGroup) New group instance.

## Discussion

            
