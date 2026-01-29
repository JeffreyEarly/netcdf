---
layout: default
title: attributes
parent: NetCDFGroup
grand_parent: Classes
nav_order: 8
mathjax: true
---

#  attributes

key-value Map of group attributes


---

## Discussion

  A `containers.Map` type that contains the key-value pairs of all
  attributes for this group. This is intended to be
  *read only*. If you need to add a new attribute to file, use
  [`addAttribute`](#addattribute).
 
  Usage
  ```matlab
  model = ncfile.attributes('model');
  ```
  
