Prepare and download Sentinel-2 data
==============================================

The tool downloads source data, prepares Sentinel-2 data and provides link to download the result.

Supported ID types are Copernicus, GoogleCloud and MPC (L2A only).

You can get ID for Copernicus catalog using the tool `Copernicus Sentinel image search <https://toolbox.nextgis.com/t/imagesearch>`_ or `Sentinel-2 scenes to GPKG <https://toolbox.nextgis.com/t/s2_search>`_.

Inputs:

* Scene identifier of Sentinel-2 (Level 1C and Level 2A). 
* Vector mask to clip the image. The format is GeoJSON, ESRI Shape (in a ZIP-archive) or any other OGR-compatible single-file format. If you don't need to clip the scene, leave this field empty.
* A list of bands. A comma separated list of numbers. The bands will be merged in the specified order, for example 4,3,2. Leave this field empty to merge all bands.
* Output spatial resolution of the scene, in meters. Leave this field empty for original spatial resolution. If number is set, then all bands will be upscaled or downscaled to it using cubic interpolation. The example of interpolation is available `here <https://docs.nextgis.com/_images/download_and_prepare_l8_s2.png>`_.


Outputs:

*  GeoTIFF output image

Launch tool: https://toolbox.nextgis.com/t/download_and_prepare_l8_s2

.. raw:: html

   <iframe width="560" height="315" src="https://www.youtube.com/embed/avKvKrsjDSI?si=5ODVonI0TYbDtw4v" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Watch on `youtube <https://youtu.be/avKvKrsjDSI?si=sJZqD5IEeZmJOxIJ>`_.

Download an example of initial data and calculation results: https://nextgis.com/data/toolbox/download_and_prepare_l8_s2/download_and_prepare_l8_s2.zip

View the result on an interactive map: https://demo.nextgis.com/resource/4805/display?panel=layers

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/download_and_prepare_l8_s2/download_and_prepare_l8_s2_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/download_and_prepare_l8_s2/download_and_prepare_l8_s2_outputs.zip>`_ to additionally check the results.

.. note:: You can download previews of the scenes using the gool `Sentinel-2 scenes to GPKG <https://toolbox.nextgis.com/t/s2_search>`_ to determine for which of them to download the full raster images.