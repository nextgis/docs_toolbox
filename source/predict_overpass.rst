Prediction of a satellite overpass
===================================

The tool forms an XLSX file with the data on Aqua, Terra, S-NPP, NOAA 20 and NOAA 21 satellites passing over an area of interest in a selected period of time.

Inputs:

* Area of interest - vector file with a polygon in GDAL-supported format, e.g. GeoPackage, GeoJSON, MapInfo TAB, ESRI Shapefile (the last two - in ZIP-archive). The area of the polygon should be no less than 200 sq. km. 
* Start date - date of the beginning of an observation. Should be in yyyy-mm-dd format.
* End date - date of the end of an observation. Should be in yyyy-mm-dd format.


.. note::
    The restriction about minimum size of the polygon is based on the high speed of satellite fly and the frequency of requests about its position (every 5 seconds). Therefore, the bigger the area of interest, the more complete will be information about satellite overpass.


Output:

* XLSX file with the date and time of the satellite overpasses.

Launch the tool: https://toolbox.nextgis.com/operation/predict_overpass

**Try it out using our sample:**

Download `input dataset <https://nextgis.ru/data/toolbox/predict_overpass/predict_overpass_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.ru/data/toolbox/predict_overpass/predict_overpass_outputs.zip>`_ to additionally check the results.
