.. todo:: Does not work, removed from tools.rst

TROPOMI to GeoTIFF
==================

The tool converts TROPOMI nitrogen dioxide data to GeoTIFF format.

Inputs:

*  TROPOMI data file in NetCDF format obtained from https://s5phub.copernicus.eu/dhus/#/home. 
   Product type: L2__NO2__, Timeliness: Offline. 
   Example of a file’s name: S5P_OFFL_L2__NO2____20190901T091635_20190901T105804_09761_01_010302_20190907T113505.nc

This dataset is available at https://browser.dataspace.copernicus.eu or ``s3://meeo-s5p/OFFL/L2__NO2___/`` (access via AWS CLI).

Outputs:

*  GeoTIFF output image

Launch the tool: https://toolbox.nextgis.com/t/tropomi2geotiff

Interactive map with the result of the tool run:

.. figure:: _static/tropomi2geotiff.png
   :align: center
   :width: 16cm

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.
