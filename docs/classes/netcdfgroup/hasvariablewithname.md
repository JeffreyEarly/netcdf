---
layout: default
title: hasVariableWithName
parent: NetCDFGroup
grand_parent: Classes
nav_order: 21
mathjax: true
---

#  hasVariableWithName

Determine whether a variable exists in this group.


---

## Discussion

  ```matlab
  bool = ncfile.hasVariableWithName('t');
  ```
 
  will return true if there exists one or more variables with
  that name.
 
  ```matlab
  bool = ncfile.hasVariableWithName('wave-vortex/t');
  ```
  
  will return true only if exactly that variable path exists.
