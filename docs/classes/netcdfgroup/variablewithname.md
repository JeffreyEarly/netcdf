---
layout: default
title: variableWithName
parent: NetCDFGroup
grand_parent: Classes
nav_order: 29
mathjax: true
---

#  variableWithName

Retrieve a variable by name or path.


---

## Declaration
```matlab
 var = variableWithName(,variableName)
```
## Parameters
+ `variableName`  (char|string) Variable name or group-qualified path.

## Returns
+ `var`  (NetCDFVariable) Matching variable object.

## Discussion

  ```matlab
  var = ncfile.variableWithName('x');
  ```
 
  var will be either NetCDFRealVariable or
  NetCDFComplexVariable.
 
        
