# GIS: Rooftop Detection Algorithm

## Overview
This is the python code for detecting rooftops from Aerial RGBD (and IR if available) data using simple image processing techniques. It uses moderate computational resources and has low interface time for segmenting rooftops. Works best on elevation data generated from photogrammetry with around 5cm ground resolution. The two inputs are the RGB (ortho-photo) and the Digital Elevation Model (DEM) geotifs. IR band data may be additionally provided for using NDVI in removing tree canopies more accurately. The shape files for the roofs and clutter in roof are generated as output.

## Dependencies
```
cv2
gdal
scipy
skimage
matplotlib
numpy
multiprocessing
osgeo
```
## Usage
```
cd GIS
python script.py
```

## Result Screenshots
![image1](https://github.com/kritiksoman/GIS/blob/master/result_screenshot/DEM.png) 
DEM consisting of rooftops.

![image2](https://github.com/kritiksoman/GIS/blob/master/result_screenshot/Ortho.png) 
Ortho-photo of rooftops.

![image2](https://github.com/kritiksoman/GIS/blob/master/result_screenshot/Roof_n_clutter.png)
The detected rooftops along with clutter.

## Author
Kritik Soman