---
layout: default
title: NetCDFGroup
has_children: false
has_toc: false
mathjax: true
parent: Class documentation
nav_order: 3
---

#  NetCDFGroup

A group of NetCDF variables, dimensions, attributes, and child groups.


---

## Declaration

<div class="language-matlab highlighter-rouge"><div class="highlight"><pre class="highlight"><code>classdef NetCDFGroup < handle</code></pre></div></div>

## Overview
 
`NetCDFGroup` represents a single NetCDF group (including the root group) and
provides a uniform interface for:
 
- Creating and registering coordinate dimensions (and their coordinate variables)
- Creating, registering, and reading variables (real and complex)
- Creating and traversing a group hierarchy
- Managing group-level (global) attributes
 
Typical usage is through `NetCDFFile`, which constructs the root group and then
exposes methods that delegate to this class.
 
           



## Topics
+ Initializing
  + [`NetCDFGroup`](/netcdf/classes/netcdfgroup/netcdfgroup.html) Create and manage a NetCDF group.
+ Accessing group properties
  + [`dump`](/netcdf/classes/netcdfgroup/dump.html) Display group contents to the command window.
  + [`id`](/netcdf/classes/netcdfgroup/id.html) of the group
  + [`name`](/netcdf/classes/netcdfgroup/name.html) of the group
  + [`parentGroup`](/netcdf/classes/netcdfgroup/parentgroup.html) parent group (may be nil)
+ Working with dimensions
  + [`addDimension`](/netcdf/classes/netcdfgroup/adddimension.html) Add a new coordinate dimension and associated coordinate variable.
  + [`dimensionPathWithName`](/netcdf/classes/netcdfgroup/dimensionpathwithname.html) Return the full group-qualified path of a dimension name.
  + [`dimensionWithID`](/netcdf/classes/netcdfgroup/dimensionwithid.html) Retrieve dimensions by NetCDF dimension ID.
  + [`dimensions`](/netcdf/classes/netcdfgroup/dimensions.html) array of NetCDFDimension objects
  + [`hasDimensionWithName`](/netcdf/classes/netcdfgroup/hasdimensionwithname.html) Determine whether a dimension exists in this group.
+ Working with variables
  + [`addFunctionHandle`](/netcdf/classes/netcdfgroup/addfunctionhandle.html) Add a lazily-evaluated variable backed by a function handle.
  + [`addVariable`](/netcdf/classes/netcdfgroup/addvariable.html) Add a real or complex variable to the group.
  + [`complexVariables`](/netcdf/classes/netcdfgroup/complexvariables.html) array of NetCDFComplexVariable objects
  + [`readVariables`](/netcdf/classes/netcdfgroup/readvariables.html) Read one or more variables from file.
  + [`readVariablesAtIndexAlongDimension`](/netcdf/classes/netcdfgroup/readvariablesatindexalongdimension.html) Read variables at a single index along a named dimension.
  + [`realVariables`](/netcdf/classes/netcdfgroup/realvariables.html) array of NetCDFVariable objects
  + [`variablePathsWithName`](/netcdf/classes/netcdfgroup/variablepathswithname.html) Return all group-qualified paths matching a variable name.
  + [`variableWithName`](/netcdf/classes/netcdfgroup/variablewithname.html) Retrieve a variable by name or path.
+ Working with groups
  + [`addDuplicateGroup`](/netcdf/classes/netcdfgroup/addduplicategroup.html) Duplicate an existing group into this group.
  + [`addGroup`](/netcdf/classes/netcdfgroup/addgroup.html) Create a new child group.
  + [`groupPath`](/netcdf/classes/netcdfgroup/grouppath.html) path of group
  + [`groupWithName`](/netcdf/classes/netcdfgroup/groupwithname.html) Retrieve a child group by name.
  + [`groups`](/netcdf/classes/netcdfgroup/groups.html) array of NetCDFGroup objects
  + [`hasGroupWithName`](/netcdf/classes/netcdfgroup/hasgroupwithname.html) Determine whether a child group exists in this group.
+ Working with global attributes
  + [`addAttribute`](/netcdf/classes/netcdfgroup/addattribute.html) Add or replace a global attribute on this group.
  + [`attributes`](/netcdf/classes/netcdfgroup/attributes.html) key-value Map of group attributes
  + [`hasAttributeWithName`](/netcdf/classes/netcdfgroup/hasattributewithname.html) Determine whether a global attribute exists on this group.
+ Other
  + [`dimensionWithName`](/netcdf/classes/netcdfgroup/dimensionwithname.html) Retrieve a dimension by name.
  + [`hasVariableWithName`](/netcdf/classes/netcdfgroup/hasvariablewithname.html) Determine whether a variable exists in this group.


---