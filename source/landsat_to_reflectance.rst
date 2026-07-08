Landsat reflectance calculation
===============================

The tool recalculates the ToA Radiance of Landsat data into reflectivity with the possibility of applying atmospheric corrections, using the DOS method.

Inputs:

* The file with the radiation intensity of one of the Landsat bands - The result of radiometric calibrations of the Landsat source data, for example, using the tool https://toolbox.nextgis.com/t/landsat_to_radiance;

* Band number - The band number corresponding to the downloaded file. Usually a number, for ETM + it can also be 6_VCID_1 and 6_VCID_2;

* Landsat Metadata File - Text file from the original Landsat data archive. Depending on the data type, it is a * MTL.txt or * .MTL file;

* Processing Result Type:

 - Default reflectance calculation (0),
 - Application of DOS atmospheric correction (1).

Outputs:

* Spectral albedo of the corresponding band in GeoTIFF format.

Spectral albedo is the main type of information that should be used in the analysis of remote sensing data. It is best suited for time series analysis. The ability to apply atmospheric corrections also improves data quality.

Supported data:

* Landsat 8 (OLI, TIRS)

* Landsat 7 (ETM+)

* Landsat 5 (TM)

* Landsat 4 (TM)

Launch the tool: https://toolbox.nextgis.com/t/landsat_to_reflectance

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

  * `Landsat radiometric calibration <https://toolbox.nextgis.com/t/landsat_to_radiance?from-related-tools=1>`_
  * `Download Landsat Analysis Ready Data (GLAD ARD) <https://toolbox.nextgis.com/t/download_glad?from-related-tools=1>`_
  * `Normalized difference index <https://toolbox.nextgis.com/t/ndi?from-related-tools=1>`_
  * `Raster calculator (GDAL) <https://toolbox.nextgis.com/t/raster_calculator?from-related-tools=1>`_
