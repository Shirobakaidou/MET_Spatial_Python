# MET_Spatial_Python

This repository is to be submitted as final project for the course MET_Spatial_Python.


The idea of this project is to go through a workflow of deriving stream/basin related morpological parameters/index from a Digital Elevation Model (DEM) by integrating needed tools into python, so that the whole workflow is executed in python.

The Workflow is divided into three parts:
1. The DEM was got using Google Earth Engine Python API; The Polygon of the basin was downloaded manually.

2. The DEM was reprojected and clipped to the geometry of the basin.

3. The morpological parameters was calculated by interacting with GRASS GIS.

However, to make it possible automatizing this workflow, there are still some problems to be solved:
* each of the three parts analysis was done in separate python environment in this project ~ they need to be united. 

* The geometry of basins could also be accessed via Earth Engine; but how to export it within python session still needs some exploring.

* The GRASS Addon 'r.basin' is able to derived many advanced morporlogical parameters, but it's quite buggy...i'm still looking for solution.


Outputs of Part-1 and Part-2 are located in the folder 'data', while a few outputs from 'r.basin' are located in the folder 'output'.
