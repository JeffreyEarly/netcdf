---
layout: default
title: NetCDFRealVariable
parent: NetCDFRealVariable
grand_parent: Classes
nav_order: 1
mathjax: true
---

#  NetCDFRealVariable

initialize a NetCDFVariable either from file or scratch


---

## Discussion

  This function is not intended to be called directly by a
  user. To create a new variable, the user should call
  `addVariable' or `initVariable' on the group or file.
 
  To initialize a variable from file you must pass the group
  and variable id, e.g.
 
  ```matlab
  aVariable = NetCDFVariable(group,id=3);
  ```
 
  To create a new variable, you must pass the group and the
  other required parameters
 
  ```matlab
  aVariable = NetCDFVariable(group,name=aName,attributes=someAttributes,type='double');
  ```
 
  class(data)
