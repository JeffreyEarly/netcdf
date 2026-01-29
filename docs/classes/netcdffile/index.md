---
layout: default
title: NetCDFFile
has_children: false
has_toc: false
mathjax: true
parent: Class documentation
nav_order: 2
---

#  NetCDFFile

Read and write NetCDF files


---

## Declaration

<div class="language-matlab highlighter-rouge"><div class="highlight"><pre class="highlight"><code>classdef NetCDFFile < NetCDFGroup</code></pre></div></div>

## Overview
 
NetCDF files are a standard file format for reading and writing data.
This class is designed to simplify the task of adding new dimensions,
variables, and attributes to a NetCDF file compared to using the
built-in `ncread` and `ncwrite` functions.
 
Typical usage patterns include:
  1) Create/open a file and obtain the root group interface.
  2) Define dimensions, then define variables referencing those
     dimensions.
  3) Attach global and variable attributes, and synchronize/close.
 
```matlab
ncfile = NetCDFFile('myfile.nc')
 
% create two new dimensions and add them to the file
x = linspace(0,10,11);
y = linspace(-10,0,11);
ncfile.addDimension('x',x);
ncfile.addDimension('y',y);
 
% Create new multi-dimensional variables, and add those to the file
[X,Y] = ncgrid(x,y);
ncfile.addVariable(X,{'x','y'});
ncfile.addVariable(Y,{'x','y'});
```
 
           



## Topics
+ Initializing
  + [`NetCDFFile`](/netcdf/classes/netcdffile/netcdffile.html) Open an existing NetCDF file or create a new file at path.
+ Accessing file properties
  + [`close`](/netcdf/classes/netcdffile/close.html) the underlying NetCDF file handle.
  + [`delete`](/netcdf/classes/netcdffile/delete.html) Destructor: close the file handle if still open.
  + [`filename`](/netcdf/classes/netcdffile/filename.html) File name (base name + extension) derived from path.
  + [`format`](/netcdf/classes/netcdffile/format.html) NetCDF format identifier.
  + [`path`](/netcdf/classes/netcdffile/path.html) File path to the NetCDF dataset.
  + [`sync`](/netcdf/classes/netcdffile/sync.html) Synchronize in-memory changes to disk.
+ Working with groups
  + [`duplicate`](/netcdf/classes/netcdffile/duplicate.html) the NetCDF dataset to a new file.


---