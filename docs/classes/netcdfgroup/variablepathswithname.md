---
layout: default
title: variablePathsWithName
parent: NetCDFGroup
grand_parent: Classes
nav_order: 28
mathjax: true
---

#  variablePathsWithName

Return all group-qualified paths matching a variable name.


---

## Declaration
```matlab
 varPaths = variablePathsWithName(grp,variableName)
```
## Parameters
+ `variableName`  (char|string) Variable name.

## Returns
+ `varPaths`  (string) Matching variable paths.

## Discussion

  ```matlab
  varPaths = ncfile.variablePathsWithName('x');
  ```
 
  
 
        
