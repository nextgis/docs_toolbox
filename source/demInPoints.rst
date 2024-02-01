Extract elevations from DEM
===========================

The extraction of elevations from DEM. Returns CSV with coordinates and altitude.

Inputs:

*  zip-compressed CSV - CSV table with coordinates of points. Delimiter should be comma. Corrdinates are floating values. File should not have spaces and should contain only latin symbols.
*  Latitude - fieldname for Latitude column. Case-sensitive.
*  Longitude - fieldname for Lonitude column. Case-sensitive.
*  Elevation dataset - choose from: gmted, gebco, alos. GMTED2010 resolution- 7.5 sec (about 250 meters), GEBCO resolution - 15 sec (about 500 meters), ALOS World 3D - 30 meters. 

Outputs:

*  zip-compressed CSV-file with coordinates and elevation values for given points.


Launch tool: https://toolbox.nextgis.com/operation/demInPoints

Download an example of initial data and calculation results: https://nextgis.ru/data/toolbox/deminpoints/deminpoints.zip
