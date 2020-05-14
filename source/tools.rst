.. sectionauthor:: Maxim Dubinin <maxim.dubinin@nextgis.com>
.. NextGIS Toolbox TOC

.. _toolbox_intro:

Tools
=====

.. _toolbox_quadro:

Set of squares generator
------------------------

This tool creates a set of square grids (polygons) and a transect of their detour for a given territory.

Inputs:

* x0 - Longitude of the anchor point
* y0 - Latitude of the anchor point
* x1 - Longitude of the reference point
* y1 - Latitude of the reference point
* size1 - Number of cells on the first axis
* size2 - Number of cells on the second axis
* side - Cell generation side (right, left)
* base_interval - The size of a cell’s side, meters

Calculation algorithm: from the anchor point in the direction of the reference point a line is drawn with a length equal to size1 * base_interval. From this line, either to the right or left of it, a second line is laid out with the length of size2 * base_interval, meters. These two lines form a grid of squares.

The result of the process is a set of layers:

* rect1 - a grid of cells the size of size1 * size2 cells, the center of the first cell is at the anchor point
* rect2 - a grid of smaller cells the size of size1 * size2 cells (i.e. 4 times larger cells, each large cell is divided into 4 parts)
* line1 - bypass lines in the direction, which if perpendicular to the line represented by the anchor point and reference point
* line2 - bypass lines in the direction, which is parallel to the line represented by the anchor point and reference point
* centers - grid cell centers rect1

Launch tool: https://toolbox.nextgis.com/operation/quadro

Download sample results: http://nextgis.ru/data/toolbox/quadro/outputs.zip

View the results on an interactive map: https://demo.nextgis.com/resource/4582/display?panel=layers

.. figure:: _static/quadro.png
   :align: center
   :width: 16cm
   
An example of the results


.. _toolbox_generalization:

Generalization of vector data
-----------------------------

Simplification of vector layer features to reduce data volume.

Inputs:

* A vector layer in ESRI Shape format, compressed(zip)
* import_snap - 
* iterations - 
* method - метод упрощения, один из: 'douglas', 'douglas_reduction', 'lang', 'reduction', 'reumann', 'boyle', 'sliding_averaging', 'distance_weighting', 'chaiken', 'hermite', 'snakes', 'displacement'.
* threshold - порог упрощения (вводится в метрах)
* look_ahead - 
* reduction - 
* slide - 
* angle_thresh - 
* alpha - 
* beta - 

The result of the process is a layer with simplified features (geometries).

Launch tool: https://toolbox.nextgis.com/operation/generalization

Download an example of source data and result: https://demo.nextgis.com/api/resource/4548/export?zipped=true&format=shp

View the result on an interactive map: https://demo.nextgis.com/resource/4108/display?panel=info

More on startup options: https://grasswiki.osgeo.org/wiki/V.generalize_tutorial

.. _toolbox_dem:

DEM data package
----------------
  
Generates elevation package.

Inputs:

* Elevation step. Integer value.
* Database. Choice from: ALOS, GMTED, GEBCO.
* Cropping boundary. Upload  compressed (zip) file in GeoJSON format (EPSG: 4326).

The result of the process is a set of layers:

* Elevation contours (isolines) with a given step
* Digital elevation model (30 m resolution, if the area is below 60 ° N, 250 m if above)
* Hillshading (same resolution as DEM)

Launch tool: https://toolbox.nextgis.com/operation/dem

Download sample results: https://demo.nextgis.com/api/resource/4548/export?zipped=true&format=shp

View the results on an interactive map: https://demo.nextgis.com/resource/4108/display?panel=info

.. figure:: _static/isolines_sample.png
   :align: center
   :width: 16cm
   
   Rendering example 

.. _toolbox_launch_conditions:


.. _toolbox_split_to_equal:

Split into equal parts
----------------------

Inputs:

* Polygon Layer (zip with Shapefile)

The result of the process is a layer:

* Polygons with approximately the same area

Launch tool: https://toolbox.nextgis.com/operation/split_to_equal

View the results on an interactive map: https://demo.nextgis.com/resource/4552/display?panel=layers


.. _toolbox_demInPoints:

Extract elevations from DEM
---------------------------

The extraction of elevations from DEM. Returns CSV with coordinates and altitude.

Launch tool: https://toolbox.nextgis.com/operation/demInPoints

.. _toolbox_lesis2sqlite:

Lesis (TopoL) to SQLite
-----------------------

Conversion of the Lesis database (TopoL-L GIS) to SQLite format to open in NextGIS QGIS.

Launch tool: https://toolbox.nextgis.com/operation/lesis2sqlite

Download an example of initial data and calculation results: http://nextgis.ru/data/toolbox/lesis2sqlite/lesis.zip


.. _toolbox_eraser:

Erase from target
-----------------

A tool that allows you to erase areas from the target layer. Areas to be erased are taken from another layer.

Inputs:

* Vector layer from which some areas are needed to be erased

ZIP archive with ESRI Shapefile or an other file format supported by OGR.

* Vector layer containing features representing areas needed to be erased from the target layer

ZIP archive with ESRI Shapefile or other file format supported by OGR.

The result of the tool’s usage is a new vector layer.

The initial vector layers must have the same coordinate system.

Launch tool: https://toolbox.nextgis.com/operation/eraser

Download an example of initial data and calculation results: http://nextgis.ru/data/toolbox/eraser/eraser.zip

View the source data and the results of calculations on an interactive map: https://demo.nextgis.com/resource/4611/display?panel=info


.. figure:: _static/eraser.png
   :align: center
   :width: 16cm

   An example of the result of the tool’s usage


.. _toolbox_change_attributes:

Change attributes in the layer group
------------------------------------

The tool changes the value of the target attribute for the selected features in the layer group in the specified Web GIS resource. Features are selected according to the set value of the selected field.

Inputs:

* Web GIS Address — The URL of your Web GIS (http(s): //***.nextgis.com)
* Login - The username of the user who has the permission to write data to the specified resource
* Password - Web GIS user password
* Resource Group Identifier - Web GIS Resource Identifier that contains layer groups
* Initial field - the name of the initial field used to search for features
* Initial value - The value of the field used to select features (identifier)
* Target field - The name of the target field, which values you want to change
* Target Value - The attribute value, which will be applied
* Start year - Starting date of the time range (optional parameter)
* End year - Ending date of the time range (optional parameter)

.. note::
    Start year and end year are optional parameters. These parameters allow you to limit the time range for the selected layers. To use these parameters, you must make sure that the time ranges are indicated in the names of the layers of the Web GIS resource. For example, in layer 1245_1246_rus_earl_v.1.0 1245 and 1246 the years are indicated. If these parameters are in use, you need to enter three or four digit values. Other parameters are **mandatory**.

Outputs:

*  A CSV file that contains data about the initial and target fields, the identifier value, the previous and new values ​​of the target field, as well as a list of hyperlinks to features that have been changed.

.. figure:: _static/result.PNG
   :align: center
   :width: 16cm

   An example of the result of the tool’s usage

Launch tool: https://toolbox.nextgis.com/operation/field_value_changer

Resource group example: https://demo.nextgis.com/resource/4793

Example of initial data:

* Web gis address = https://demo.nextgis.com
* Login = *****
* Password = *****
* Resource Group Id = 4793
* Initial field = fid
* Initial value = 1216
* Target field = fid2
* Target valuе = 1112
* Start Year = 1244
* End Year = 1300


.. _toolbox_raster_calculator:

Raster calculator
-----------------

.. figure:: _static/raster_calculator.png
   :align: center
   :width: 16cm
   
   
A tool that implements raster arithmetics for multi-band rasters or groups of single-band rasters.

Inputs:

* Initial raster data

The initial raster data can be presented in two forms:

1. Multi-band raster in GDAL-compatible format

2. ZIP archive with a set of single-bandl GDAL-compatible rasters

Rasters in the archive can be stored in different coordinate systems, have different extents and cell sizes. When calculated, everything will be reduced to a single spatial domain.

* Expression.

Standard expression using the operators +, -, *, /,>, <, etc. If the initial data is in a ZIP archive, then the names of the source files in the expression should be used (for example, band4.tif / band5.tif, if the files have the corresponding names). The extension is part of the name. 
For a multi-band raster, use the band number with the & prefix (for example, & 4 / & 5). Bands are numerated starting at 1.

Examples of expressions:

Forest areas with a temperature of less than 30 degrees:

forest_mask.tif * (land_temperature.tif < 30)


EVI Index:

2.5 * (&5 - &4) / (&5 + 6.0*&4 - 7.5*&2 + 1.0)


* The name of the resulting raster

No file extension (e.g. ndvi, water). The extension will be automatically set to .tif

* X resolution

The width of each individual pixel in the resulting raster in the coordinate system units of the first raster from the set (eg 30). Use the - symbol to automatically select the pixel width

* Y resolution

The height of each individual pixel in the resulting raster in the coordinate system units of the first raster from the set (eg 30). Use the - symbol to automatically select the pixel height

* The extent of the resulting raster

Format: xmin, ymin, xmax, ymax. Example: 1000, 1000, 2500, 2500. Use - to automatically determine the extent. In this case, the intersection extent of all input rasters will be calculated

* Data Type for a New Raster

Available data types: Int32, Int16, Float64, UInt16, Byte, UInt32, Float32. Use - to automatically select the data type.

The result of the process is a single-band raster in the GeoTiff format, calculated according to the specified expression.

If the user sets one of the optional parameters (resolution along one of the axes or the extent), then first all the rasters involved in the expression are brought to the specified state, when the calculations are performed. In case of an automatic selection of spatial domain parameters the following logic is used:

1. The lowest spatial resolution among all source rasters is calculated. It is taken as an output.

2. All rasters are reprojected on the coordinate system of the first raster in the list.

3. The output extent is calculated as the extent of the intersections of all the initial rasters.



Launch tool: https://toolbox.nextgis.com/operation/raster_calculator

Download an example of initial data (multi-band raster, 11 bands, a fragment of the Landsat 8 scene): http://nextgis.ru/data/toolbox/raster_calculator/LC08_B1_B11.TIF

Download an example of initial data (archive with rasters, fragments of the Landsat 8 scene, available in the name expression: band2.tif, band3.tif, band4.tif, band5.tif, band3_cropped.tif): http://nextgis.ru/data/ toolbox / raster_calculator / LC08_20180530.zip

Download examples of calculation results:

* For example with the archive (NDVI calculation). Expression: (band5.tif - band4.tif) / (band5.tif + band4.tif). File: http://nextgis.ru/data/toolbox/raster_calculator/ndvi.tif

* For example with a multi-band raster (masking a section of a river). Expression: ((& 5 - & 4) / (& 5 + & 4)) <-0.12. File: http://nextgis.ru/data/toolbox/raster_calculator/water_mask.tif


View source data and calculation results on an interactive map: https://demo.nextgis.com/resource/4566/display?panel=info


.. _toolbox_prepare_raster:

Prepare raster
--------------
   
A tool that performs a per-band connection of a set of single-band rasters and crops the result using a vector mask.

Input:

* Initial raster data

The initial raster data can be presented in two forms:

1. Multi-band raster in GDAL-compatible format

2. ZIP archive with a set of single-baned GDAL-compatible rasters

* Vector layer, which is used as mask

ZIP archive with ESRI Shapefile or a other file format supported by OGR.

* “No data” value

The value that is marked as “No data”. Use the - symbol to use the default value.

* The name of the resulting raster

No file extension (e.g. ndvi, water). The extension will be automatically installed in .tif

If the input is an archive with single-band rasters, the tool first combines them into a multi-band raster. The order of the bands is determined by alphabetically sorting the names of the initial rasters in the archive. 
Then the multi-band raster (assembled from the archive or submitted immediately) is cropped with a vector mask.

The initial rasters and the vector mask can be in different coordinate systems before processing, all data is brought into a single spatial domain.

Launch tool: https://toolbox.nextgis.com/operation/prepare_raster

Download an example of initial data and calculation results: http://nextgis.ru/data/toolbox/prepare_raster/prepare_raster.zip

View the source data and calculation results on the interactive map: https://demo.nextgis.com/resource/4595/display?panel=info

.. figure:: _static/prepare_raster.png
   :align: center
   :width: 16cm

   An example of the result of the tool’s usage

.. _toolbox_landsat_to_radiance:

Landsat radiometric calibration
-------------------------------
   
The tool converts the Landsat raw data into radiation intensity (ToA Radiance).

Inputs:

* Landsat band initial File

Processing level L1 file from the original Landsat data archive. The name can be anything. Data can be pre-trimmed, etc.

* Band number

The band number corresponding to the downloaded file. Usually a number, for ETM + it can also be 6_VCID_1 and 6_VCID_2

* Landsat Metadata File

Text file from the original Landsat data archive. Depending on the data type, it is a * MTL.txt or * .MTL file.

Outputs:

* The radiation intensity of the corresponding band in the GeoTIFF format

Radiometric calibration is necessary for time series analysis, calculation of derivative products (for example, index images).

Supported data:

* Landsat 8 (OLI, TIRS)

* Landsat 7 (ETM+)

* Landsat 5 (TM)

* Landsat 4 (TM)

Launch tool: https://toolbox.nextgis.com/operation/landsat_to_radiance

Download an example of source data and calculation results: http://nextgis.ru/data/toolbox/landsat_to_radiance/landsat_to_radiance.zip

.. _toolbox_landsat_to_reflectance:

Landsat reflectance calculation
-------------------------------
   
The tool recalculates the ToA Radiance of Landsat data into reflectivity with the possibility of applying atmospheric corrections, using the DOS method.

Inputs:

* The file with the radiation intensity of one of the Landsat bands

The result of radiometric calibrations of the Landsat source data, for example, using the tool https://toolbox.nextgis.com/operation/landsat_to_radiance

* Band number

The band number corresponding to the downloaded file. Usually a number, for ETM + it can also be 6_VCID_1 and 6_VCID_2

* Landsat Metadata File

Text file from the original Landsat data archive. Depending on the data type, it is a * MTL.txt or * .MTL file

* Processing Result Type

0 for calculating the default albedo, 1 for applying atmospheric corrections using the DOS method

Outputs:

* Spectral albedo of the corresponding band in GeoTIFF format

Spectral albedo is the main type of information that should be used in the analysis of remote sensing data. It is best suited for time series analysis. The ability to apply atmospheric corrections also improves data quality.

Supported data:

* Landsat 8 (OLI, TIRS)

* Landsat 7 (ETM+)

* Landsat 5 (TM)

* Landsat 4 (TM)

Launch tool: https://toolbox.nextgis.com/operation/landsat_to_reflectance

Download an example of source data and calculation results: http://nextgis.ru/data/toolbox/landsat_to_reflectance/landsat_to_reflectance.zip

.. _toolbox_ndi:

Normalized difference index
---------------------------
   
The tool calculates the normalized difference index for any two input images.

Inputs:

* First component of the difference index

Any GDAL-compatible raster

* Second component of the difference index

Any GDAL-compatible raster

Outputs:

* A raster with normalized difference index in GeoTiff format

The calculation is carried out according to the formula: (First image - Second image) / (First image + Second image). The pixel values of the resulting raster are in the range from -1 to 1
Before the calculation, both images are brought into a single spatial domain. The projection and spatial resolution of the first raster is used.

Examples of common normalized difference indices:

* NDVI - for vegetation assessment (the first raster - NIR, the second - RED) For Landsat 8 data: 5 and 4 bands.
* NDWI - for the detection of water bodies (the first raster - NIR, the second - SWIR). For Landsat 8 data: 5 and 6 bands.
* NDSI - for assessing the snow cover (the first raster - GREEN, the second - SWIR). For Landsat 8 data: 3 and 6 bands.

Launch tool: https://toolbox.nextgis.com/operation/ndi

Download an example of source data and calculation results: http://nextgis.ru/data/toolbox/ndi/ndi.zip

.. _toolbox_ogrmerge:
 
Merge vector layers
-------------------
   
.. figure:: _static/ogrmerge.png
   :align: center
   :width: 16cm

   Initial and resulting data
   
The tool merges many vector layers into one.

Inputs:

* ZIP archive with .shp, .geojson, .gpkg, .tab files

Outputs:

* GeoPackage file with the result of the merge

The tool has no limit on the number of initial layers. The name of the source layer is not saved.

Launch tool: https://toolbox.nextgis.com/operation/ogrmerge

Download an example of initial data and calculation results: http://nextgis.ru/data/toolbox/ogrmerge/ogrmerge.zip

.. _toolbox_ngw_copy_layer:
 
Duplicate nextgis.com vector layer
----------------------------------
   
.. figure:: _static/ngw_copy_layer.png
   :align: center
   :width: 16cm

   Initial and resulting data
   
The tool duplicates the structure of the nextgis.com vector layer into another directory or instance. Field names, field order, field types, aliases, and descriptions are copied. Metadata in the current version are not copied.

Inputs:

*  Two pairs of URLs, usernames and passwords, id of the initial layer and id of the new folder

Outputs:

* There is no output, the result is the creation of a layer in nextgis.com

Features: Suitable for layers created by NextGIS FormBuilder. Used in the process of layer replication. Data is not copied.

Launch tool: https://toolbox.nextgis.com/operation/ngw_copy_layer

Download an example of source data and calculation results: http://nextgis.ru/data/toolbox/ngw_copy_layer/ngw_copy_layer.zip


.. _toolbox_kpt2geo:
 
Convert EGRN KPT to geodata
---------------------------
   
.. figure:: _static/kpt2geo.png
   :align: center
   :width: 16cm

   Initial and resulting data
   
The tool converts one or several Rosreestr KPT from XML format into a convenient geodata format with a GIS project.

Inputs:

*  Zip archive with zip archives of Rosreestr downloads (archive of archives with the name format Response-80-105152635.zip)
*  Output geodata format - GeoJSON, ESRI Shape, Mapinfo TAB

Outputs:

* zip archive with the QGIS project and geodata

The archive contains directories: a geodata directory in the local coordinate system (msk), a geodata directory in EPSG: 4326 (wgs) and a project for QGIS with data in EPSG: 4326 with the design.

A description of the layers is given at https://data.nextgis.com/en/cadastre/#region-layers

Launch tool: https://toolbox.nextgis.com/operation/pkk_kpt

Download an example of initial data and calculation results: http://nextgis.ru/data/toolbox/kpt2geo/kpt2geo.zip


.. _toolbox_ai2geo:

Adobe Illustrator (*.ai) to geodata
-----------------------------------

The tool extracts vector data layers from an Adobe Illustrator (* .ai) file using an additional file in GeoTIFF format for georeference.

Inputs:

* An Adobe Illustrator file (with the .ai extension) that contains vector features 
* A GeoTIFF file (with the extension .geotiff or .tif), on the basis of which the georeferencing of the extracted vector features will be performed

The tool works in the following way: geometries are extracted from the .ai file. For each geometry, its type (point, line or polygon) is determined, as well as the style with which it is drawn (line thickness, line color, fill color). Layers are created (according to the types of geometries) in which each feature will contain the resulting geometry and a style string in the “STYLE” field. In this case, the coordinates of the geometries are converted from local coordinates to spatial coordinates, based on the transmitted GeoTIFF file, which must contain the correct geospatial reference (it is implied, that the vector features in the .ai file were drawn “on top” of a similar image in Adobe Illustrator).

The result of the process is a ZIP archive containing a set of files in the ESRI Shapefile format according to the created layers.

Launch tool: https://toolbox.nextgis.com/operation/ai2geo

.. figure:: _static/ai2geo_before.png
   :align: center
   :width: 32cm
   
   Source vector data in .ai file

.. figure:: _static/ai2geo_after.png
   :align: center
   :width: 32cm
   
   The result of the tool’s usage: the resulting layers are loaded into QGIS and displayed on the background of the OSM basemap

.. _toolbox_grid:
 
Meter grid
----------
   
.. figure:: _static/grids-demo.png
   :align: center
   :width: 16cm

   Generated grid
   
The tool generates a grid within the boundaries of features of a vector layer. The grid size is set in meters. Features can be anywhere in the world.

Inputs:

*  A multipolygon layer with one or more features. It can be in any format opened by OGR (GeoPackage, geojson)
*  Grid step in meters
*  Mode: points (points), rect (squares)
*  Algorithm for cropping the grid along the borders: all (leave all the squares in extent), touches (leave all the squares touching features), intersection (crop the squares along the borders of the features)

.. figure:: _static/grid-1000-rect-all.png
   :align: center
   :width: 16cm

   all
   
   
.. figure:: _static/grid-1000-rect-touches.png
   :align: center
   :width: 16cm

   touches
   
   
.. figure:: _static/grid-1000-rect-intersection.png
   :align: center
   :width: 16cm

   intersection
   
   
.. figure:: _static/grid-1000-point-all.png
   :align: center
   :width: 16cm

   all для точек
   
   
.. figure:: _static/grid-1000-point-intersection.png
   :align: center
   :width: 16cm

   touches и intersection для точек

   
.. figure:: _static/grid-planet.png
   :align: center
   :width: 16cm

   Generated grids for several polygons in different places of the globe
   

*  output geodata format - GeoJSON, ESRI Shape, Mapinfo TAB

Outputs:

* Geopackage


Launch tool: https://toolbox.nextgis.com/operation/grid



.. _toolbox_last_img:
 
Last GEE imagery
----------------
   
The tool requests an image’s metadata of the user-specified Google Earth Engine image collection (images are analyzed within a fixed area), starting from a given date.

Inputs:

*  The name of the collection in GEE format (for example, LANDSAT / LC08 / C01 / T1_SR)
*  Start date: collection images created earlier than this date are ignored. Metadata is returned from images created later than the date. Date format: YYYY-MM-DD
*  The archive (zip) of the GEE access file can usually be found in the user's home directory (.config / earthengine / credentials)

Outputs:

*  Metadata for requested images
*  The output data format is JSON (packed in zip)

Launch tool: https://toolbox.nextgis.com/operation/last_img


.. _toolbox_download_and_prepare_l8_s2:
 
Download and clip Landsat 8 / Sentinel 2 data
---------------------------------------------
   
The tool downloads and prepares Landsat-8 / Sentinel-2 data.

Inputs:

*  Landsat 8 / Sentinel 2 scene identifier, data type is determined automatically by the identifier. You can get the identifier, for example, at https://earthexplorer.usgs.gov
*  The vector mask, which will crop the image. The format is GeoJSON, ESRI Shape (in a zip archive) or any other OGR-compatible file
*  A list of bands. A comma separated list of numbers. The bands will be merged in the specified order, for example 2,3,4. Use - to load and merge all bands


Outputs:

*  GeoTIFF output image

Launch tool: https://toolbox.nextgis.com/operation/download_and_prepare_l8_s2

Download an example of initial data and calculation results: http://nextgis.ru/data/toolbox/download_and_prepare_l8_s2/download_and_prepare_l8_s2.zip

View the result on an interactive map: https://demo.nextgis.com/resource/4805/display?panel=layers

Examples of initial data:

*  Scene S2A_MSIL1C_20191109T072121_N0208_R006_T41VLD_20191109T084554
* Bands 4.3.2
*  File

```
{
"type": "FeatureCollection",
"name": "ekb",
"crs": { "type": "name", "properties": { "name": "urn:ogc:def:crs:OGC:1.3:CRS84" } },
"features": [
{ "type": "Feature", "properties": { }, "geometry": { "type": "Polygon", "coordinates": [ [ [ 60.46, 56.77 ], [ 60.7, 56.77 ], [ 60.7, 56.92 ], [ 60.46, 56.92 ], [ 60.46, 56.77 ] ] ] } }
]
}
```

.. _tropomi2geotiff:
 
TROPOMI to GeoTIFF
------------------
   
The tool converts TROPOMI nitrogen dioxide data to GeoTIFF format.

Inputs:

*  TROPOMI data file in NetCDF format obtained from https://s5phub.copernicus.eu/dhus/#/home. Product type: L2__NO2__, Timeliness: Offline. Example of a file’s name: S5P_OFFL_L2__NO2____20190901T091635_20190901T105804_09761_01_010302_20190907T113505.nc


Outputs:

*  GeoTIFF output image

Launch tool: https://toolbox.nextgis.com/operation/tropomi2geotiff

Download an example of initial data and calculation results: http://nextgis.ru/data/toolbox/tropomi2geotiff/tropomi2geotiff.zip

View an example result on an interactive map: https://demo.nextgis.com/resource/4698/display?panel=layers

.. figure:: _static/tropomi2geotiff.png
   :align: center
   :width: 16cm
   
The source scenes are supposed to be hosted on scihub.copernicus (https://scihub.copernicus.eu) in the future, but temporarily they are hosted on a copy of the Sentinel-5P Pre-Operations Hub web interface: https://s5phub.copernicus.eu/dhus/#/ home. Logins from scihub do not work, you need to use s5pguest / s5pguest. 
   
.. _mt2report:
 
Create marine traffic report
----------------------------

This tool generates a table (format - CSV), which lists the ships entering given territory, the date and coordinates of their last location, as well as the number of times each ship entered a given territory for a certain period of time. It makes sense to use this tool, if you have already configured a service that updates data on ship locations in your Web GIS.

Inputs:

* name - Web GIS Name
* layer_id_border - zone resource ID
* layer_id_ships - ship data resource ID
* date - Start date

Calculation algorithm: Uploading layers of the boundary of the analysis zone and ship locations. Checking each location for intersection with the analysis zone; locations registered later than the specified starting date are also selected. Among the selected locations for each ship the last location and its coordinates, as well as the total number of locations are obtained. The information obtained for each ship is recorded in a table. 

The result of the process is a table in CSV format with information about all ships registered on a given territory later than the specified date, information about the last registered location and the number of registered locations within a given territory for a certain period of time.

Launch tool: https://toolbox.nextgis.com/operation/mt2report

View an example of initial data on an interactive map: https://demo.nextgis.com/resource/4693/display?panel=layers

.. figure:: _static/mt2report_map.png
   :align: center
   :width: 16cm
   
   Initial Data Example
   
.. figure:: _static/mt2report_table.png
   :align: center
   :width: 16cm
   
   An example of the result of the tool’s usage 

.. _toolbox_ngw_intersect:

Intersector
-----------

The tool intersects all layers of the nextgis.com web map using the specified geometry and generates a report listing the layers, with which the intersection took place. If different features intersect in a separate layer, these cases are displayed as separate events in the report.

Inputs:

*  url - address of the used Web GIS
*  webmap_id - web map ID from used Web GIS
*  wkt - geometry with which the intersection of layers of the web map is checked. Indicated in wkt format, coordinate system - EPSG: 3857

Outputs:

*  .xlsx table with a list of intersected layers

Launch tool: https://toolbox.nextgis.com/operation/ngw-intersect

Usage example:

How many types of anemones can you find on the Appalachian Trail?

*  url - http://demo.nextgis.com
*  webmap_id - 4714 (since the web map address is https://demo.nextgis.com/resource/4714/display)
*  wkt - LineString (-9378421.57282677479088306 4115819.42546373652294278, -7678593.31173497438430786 5764332.11640937067568302)	
 
.. figure:: _static/ngw_intersect_layers.png
   :align: center
   :width: 16cm
   
   Initial Data Example
   
.. figure:: _static/ngw_intersect_result.png
   :align: center
   :width: 16cm
   
   An example of the result of the tool’s usage 
   
.. _toolbox_lines2polygons:

Temporal polygons from lines and points
---------------------------------------

The tool creates polygons that reflect the state of the area at a particular point in time. Polygons are formed from a set of polylines, each of which is characterized by the start and end dates of its existence. Attributes for polygons are assigned from a layer of points, which also has a time reference.

In addition, grouping of polygon identifiers by a given parameter is carried out by creating a separate field with an ID common to each group (its minimum value). The geometry of the polygons does not change.

Inputs:

*  gis_url - address of the used Web GIS
*  lines_id - ID of the polyline layer from the used Web GIS
*  points_id - ID of the layer with points from the used Web GIS
*  Requested year - the year for which you want to get a time slice
*  year_field - name of the field where the requested year will be written
*  Result field - a new field where the grouping results will be entered, that is, ID
*  Field with identifiers - a field with unique values in the polyline layer; IDs for grouping are borrowed from it 
*  Grouping field - the field by which polygons are grouped

Outputs:

*  a layer with polygons (shapefile) relevant for the given year

Launch tool: https://toolbox.nextgis.com/operation/lines2polygons

Usage example:

What are the borders of the European states for the 1000th year of n. e.?

*  gis_url - https://demo.nextgis.com
*  lines_id - 4702 (as the address of the layer with polylines https://demo.nextgis.com/resource/4702/feature/)
*  points_id - 4700 (since the address of the layer with points is https://demo.nextgis.com/resource/4700/feature/)
*  The requested year - 1000
*  year_field - Year
*  Result Field - Result
*  Field with identifiers - fid_europe 
*  Grouping field - linecomnt
 
.. figure:: _static/lines2polygons_lines_points_map.png
   :align: center
   :width: 16cm
   
   Sample input data. Layers of polylines and dots 
   
.. figure:: _static/lines2polygons_lines_table.png
   :align: center
   :width: 16cm
   
   Sample input data. Polyline Layer Attributes Table  
   
.. figure:: _static/lines2polygons_polygons_map_table.png
   :align: center
   :width: 16cm
   
   An example of the result of a tool    

.. _toolbox_temporal_split:

Create temporal cache
---------------------

The tool creates several layers from one. Each new layer is a selection of features for a period of time.

Inputs:

* gis_url - address of the used Web GIS
* resource_id - ID of the polyline layer used by Web GIS
* upper_field - date the feature disappeared
* lower_field - date the feature appeared
* year1_field - the start year of the interval
* year2_field - the end year of the interval
* Date Format - date format for dates
* The output format is GeoJSON, GPKG, CSV, ESRI Shapefile (the default value is ESRI Shapefile)
* Ignore errors - leave blank to stop completion if an empty range is found. Enter 1 to ignore errors

Outputs:

*  archive of layers, each of which is also in an archive (zip)

Launch tool: https://toolbox.nextgis.com/operation/temporal_split

Usage example:

Make a temporary cache from the layer of cities appearing and disappearing at a certain time.

* Web GIS URL - https://demo.nextgis.com
* Source Resource ID - 4719
* upper_field - upperdat
* lower_field - lwdate
* year1_field - YEAR1
* year2_field - YEAR2
* Date format - 
* Output format -
* Ignore Errors - 1

Download sample results: http://nextgis.ru/data/toolbox/toolbox_temporal_split/toolbox_temporal_split.zip

.. _toolbox_poly2explication:

Polygon explication (forestry)
------------------------------

Generating a report of explication of forest plots. Used to automatically obtain a table of lengths and azimuths from a polygon.

Inputs:

* Polygonal layer (forest plot) - a vector data set (plot boundaries) in the format supported by OGR. Shape-files are transferred in an archive, single-file sets - uncompressed. There should be only 1 feature on the layer
* Line layer (reference) - Vector data set (reference) in the format supported by OGR. Shape-files are transferred in an archive, single-file sets - uncompressed. There should be only 1 feature on the layer. If the reference section can not be filled out, the “Stub” can be used instead, which is a layer without features. A stub can be taken at http://nextgis.ru/data/toolbox/poly2explication/empty_line.geojson
* Description of the binding method - free text
* Forestry number - integer

Outputs:

*  Excel report (xlsx)

Launch tool: https://toolbox.nextgis.com/operation/poly2explication

Download an example of initial data and calculation results: http://nextgis.ru/data/toolbox/poly2explication/poly2explication.zip

.. figure:: _static/poly2explication-1.png
   :align: center
   :width: 16cm
   
   An example of the result of the tool’s usage 
   
Projection (Dae, Collada) to Shapefile
--------------------------------------

The tool makes a projection of three-dimensional features on the earth's surface.

Inputs:

* Zip archive containing * .kmz and * .dae files
* *.kmz must contain the geolocation of * .dae models (coordinates of polygons in EPSG: 4326, units of measurement are metric)

Outputs:

*  A zip archive with Shapefile
*  In the resulting Shapefile for each model, the attributes “name” and “altitude” are added

You can submit several models, each of them gets a separate polygon.

Launch tool: https://toolbox.nextgis.com/operation/kmldae2footprints

Download an example of initial data and calculation results: http://nextgis.ru/data/toolbox/kmldae2footprints/kmldae2footprints.zip

Join layer and table by field
-----------------------------

The tool combines data from a table and a layer using a given field. The tool involves the use of two different join types: one-to-one - finds the first matching element of the table and attaches its attributes; one-to-many - connects all elements of the table for which the given field matches, the geometry of the feature is duplicated for each element.

Inputs:

* gis_url - address of the used Web GIS
* resource_id - layer ID to combine from the currently used Web GIS
* src - table name
* layer_field - the name of the field in the Web GIS layer
* csv_field - field name in the table
* join_type - type of join (1 - one-to-one, 0 - one-to-many)

Outputs:

*  layer in ESRI Shapefile format, which is in an archive (zip)

Launch tool: https://toolbox.nextgis.com/operation/join_by_field

Usage example:

.. figure:: _static/join_by_field.png
   :align: center
   :width: 16cm

Download sample results: http://nextgis.ru/data/toolbox/join_by_field/join_by_field.zip

Clip PBF file by bbox
---------------------

The tool downloads PBF (openstreetmap format - https://wiki.openstreetmap.org/wiki/RU:PBF_Format) and crops it along the Bounding Box (bbox) border. 

Inputs:

*  The url where the pbf file is located. Example - http://download.geofabrik.de/europe/malta-latest.osm.pbf (Malta, 4 Mb)
*  Bounding Box in CSV format. Example - 14.5013,35.887,14.5066,35.899 (coordinates of the lower left and upper right corner of the frame). The bbox line can be taken here - https://boundingbox.klokantech.com/ 
 
Outputs:

*  Bounding Box cropped pbf file

Launch tool: https://toolbox.nextgis.com/operation/osmclip_bbox

Change geometry for a group of layers
------------------------------------

The tool changes the geometry of features in a layer group of the Web GIS resource. The change is possible in 3 modes: Delete, Insert, Replace. In delete mode, the tool deletes the selected features. The selection is based on the specified values of a layer’s attribute field. In insert mode, the tool adds new features from the uploaded shp file, the structure of the file and the layer must match. Otherwise, the tool will not be able to add new features. 
In replacement mode, the tool replaces the geometry value for features from the uploaded shp file, the values of the specified attribute of which match with the attribute values of the Web GIS layer. The attribute name in the shp file and the Web GIS layer must match.

Inputs:

* Web GIS Address — The URL of your Web GIS (http (s): //***.nextgis.com)
* Login - The username of the user who has the permission to write data to the specified resource
* Password - Web GIS user password
* Resource Group Identifier - Web GIS Resource Identifier for a layer group
* Initial field - Name of the initial field used to search for features
* Mode - A type of mode, which changes the geometry of features. To delete features, select the Delete mode, to Add - insert, to Change - replace
* Initial value - The value of the field by which the features are selected. If you need to specify multiple values, use a comma to separate
* Start year - Starting date of the time range (optional parameter)
* End year - Ending date of the time range (optional parameter)
* SHP file - An ESRI Shapefile (zipped) that contains features. Required parameter in Add and Change modes

.. note::
    Start year and end year are optional parameters. These parameters allow you to limit the time range for the selected layers. To use these parameters, you must make sure that the time ranges are indicated in the names of the layers of the Web GIS resource. For example, in layer 1245_1246_rus_earl_v.1.0 1245 and 1246 the years are indicated. If these parameters are in use, you need to enter three or four digit values. Other parameters are **mandatory**.

Outputs:

*  A CSV file that contains data on the selected mode, the source field and its value, a list of hyperlinks to features that have been changed, in case of errors they will also be indicated in this file.

.. figure:: _static/geometry_changer.PNG
   :align: center
   :width: 16cm

   Launch tool: https://toolbox.nextgis.com/operation/geometry_changer
