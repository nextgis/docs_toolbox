Landsat radiometric calibration
===============================

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

Download an example of source data and calculation results: https://nextgis.ru/data/toolbox/landsat_to_radiance/landsat_to_radiance.zip
