Landsat reflectance calculation
===============================

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

**Try it out using our sample:**

Download `input dataset <https://nextgis.ru/data/toolbox/landsat_to_reflectance/landsat_to_reflectance_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.ru/data/toolbox/landsat_to_reflectance/landsat_to_reflectance_outputs.zip>`_ to additionally check the results.
