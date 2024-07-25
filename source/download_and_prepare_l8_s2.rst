Prepare satellite data and download the result
==============================================

The tool downloads source data, prepares Sentinel-2 data and provides link to download the result.

Inputs:

* Scene identifier of Sentinel-2 (Level 1C and Level 2A). You can get ID from https://dataspace.copernicus.eu/browser/, but only authorized users can search for data. You can download and explore instruction on registration and search performing :download:`here <files/sentinel_instruction_en.pdf>`
* Vector mask to clip the image. The format is GeoJSON, ESRI Shape (in a ZIP-archive) or any other OGR-compatible file. If you don't need to clip the scene, leave this field empty.
* A list of bands. A comma separated list of numbers. The bands will be merged in the specified order, for example 4,3,2. Leave this field empty to merge all bands.
* Output spatial resolution of the scene, in meters. Leave this field empty for original spatial resolution. If number is set, then all bands will be upscaled or downscaled to it using cubic interpolation. The example of interpolation is available `here <https://docs.nextgis.ru/_images/download_and_prepare_l8_s2.png>`_.


Outputs:

*  GeoTIFF output image

Launch tool: https://toolbox.nextgis.com/operation/download_and_prepare_l8_s2

Download an example of initial data and calculation results: https://nextgis.ru/data/toolbox/download_and_prepare_l8_s2/download_and_prepare_l8_s2.zip

View the result on an interactive map: https://demo.nextgis.com/resource/4805/display?panel=layers

**Try it out using our sample:**

Download `input dataset <https://nextgis.ru/data/toolbox/download_and_prepare_l8_s2/download_and_prepare_l8_s2_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.ru/data/toolbox/download_and_prepare_l8_s2/download_and_prepare_l8_s2_outputs.zip>`_ to additionally check the results.
