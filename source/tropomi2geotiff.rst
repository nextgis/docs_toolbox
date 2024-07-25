TROPOMI to GeoTIFF
==================

The tool converts TROPOMI nitrogen dioxide data to GeoTIFF format.

Inputs:

*  TROPOMI data file in NetCDF format obtained from https://s5phub.copernicus.eu/dhus/#/home. 
   Product type: L2__NO2__, Timeliness: Offline. 
   Example of a file’s name: S5P_OFFL_L2__NO2____20190901T091635_20190901T105804_09761_01_010302_20190907T113505.nc


Outputs:

*  GeoTIFF output image

Launch tool: https://toolbox.nextgis.com/operation/tropomi2geotiff

View an example result on an interactive map: https://demo.nextgis.com/resource/4698/display?panel=layers

.. figure:: _static/tropomi2geotiff.png
   :align: center
   :width: 16cm
   
The source scenes are supposed to be hosted on scihub.copernicus (https://scihub.copernicus.eu) in the future, but temporarily they are hosted on a copy of the Sentinel-5P Pre-Operations Hub web interface: https://s5phub.copernicus.eu/dhus/#/ home. Logins from scihub do not work, you need to use s5pguest / s5pguest. 

**Try it out using our sample:**

Download `input dataset <https://nextgis.ru/data/toolbox/tropomi2geotiff/tropomi2geotiff_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.ru/data/toolbox/tropomi2geotiff/tropomi2geotiff_outputs.zip>`_ to additionally check the results.
