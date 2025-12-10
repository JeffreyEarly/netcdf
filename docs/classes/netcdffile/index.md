---
layout: default
title: NetCDFFile
has_children: false
has_toc: false
mathjax: true
parent: Class documentation
nav_order: 1
---

#  NetCDFFile

A class for reading and writing to NetCDF files


---

## Declaration

<div class="language-matlab highlighter-rouge"><div class="highlight"><pre class="highlight"><code>classdef NetCDFFile < NetCDFGroup</code></pre></div></div>

## Overview
 
  NetCDF files are a standard file format for reading and writing data.
  This class is designed to simplify the task of adding new dimensions,
  variables, and attributes to a NetCDF file compared to using the
  built-in `ncread` and `ncwrite` functions.
 
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
  + [`NetCDFFile`](/netcdf/classes/netcdffile/netcdffile.html) initialize an from existing or create new file
+ Accessing file properties
  + [`format`](/netcdf/classes/netcdffile/format.html) format
  + [`path`](/netcdf/classes/netcdffile/path.html) file path the NetCDF file
+ Other
  + [`close`](/netcdf/classes/netcdffile/close.html) - Topic: Accessing file properties
  + [`delete`](/netcdf/classes/netcdffile/delete.html) 
  + [`duplicate`](/netcdf/classes/netcdffile/duplicate.html) 
  + [`filename`](/netcdf/classes/netcdffile/filename.html) 
  + [`sync`](/netcdf/classes/netcdffile/sync.html) - Topic: Accessing file properties


---