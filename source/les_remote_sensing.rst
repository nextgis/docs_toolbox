Prepare satellite data and upload it to Web GIS
===============================================

The tool allows you to get a Sentinel-2 scene by its ID, crop it by the input vector mask and upload it to Web GIS with automatically created style.

Inputs:

*  Scene identifier of Sentinel 2 (Level 1C and Level 2A). You can get ID from https://dataspace.copernicus.eu/browser/, but only authorized users can search for data. You can download and explore instruction on registration and search performing :download:`here <files/sentinel_instruction_en.pdf>`
*  Vector mask to clip the scene. Possible formats - GeoJSON, ESRI Shape (in ZIP archive) or any other OGR-supported file. If you need the whole scene, just leave this field empty.
*  Output spatial resolution of the scene, in meters. Leave this field empty for original spatial resolution. If number is set, then all bands will be upscaled or downscaled to it using cubic interpolation. The example of interpolation is available `here <https://docs.nextgis.com/_images/download_and_prepare_l8_s2.png>`_.
*  URL of Web GIS which will host processed scene.
*  Login for Web GIS which will host processed scene.
*  Password for Web GIS which will host processed scene.
*  Identifier of the parent Web GIS resource (folder) to which processed scene will be uploaded. Please specify the number corresponding to target resource, you can find it in address bar of the browser. For instance, corresponding number for resource “Examples” is 3880 since its address is  https://demo.nextgis.com/resource/3880
*  Use naming convention for Les – applicable only for NextGIS Les app users, please ignore. 

Outputs:

*  GeoTIFF of processed scene and its style uploaded to Web GIS.

Launch tool: https://toolbox.nextgis.com/operation/les_remote_sensing

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/les_remote_sensing/les_remote_sensing_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/les_remote_sensing/les_remote_sensing_outputs.zip>`_ to additionally check the results.
