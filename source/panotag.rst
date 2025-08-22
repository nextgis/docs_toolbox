Add Google Photosphere XMP metadata to photos
=============================================

Sometimes spherical panoramic images don't have the neccessary tags which stops the viewers from displaying them correctly. This tool adds XMP tags corresponding to the `specification <https://developers.google.com/streetview/spherical-metadata>`_ that notify the viewing widget that:

* it's a spherical panoramic image;
* FOV is 360x180.

So the input image must indeed have 360x180 field of view.

GPano:PoseHeadingDegrees is copied from GPSImgDirection.

Inputs:

* ZIP with photos.

Outputs:

* ZIP with modified photos with added tags.

You can `add spherical panoramas to features on a Web Map <https://docs.nextgis.com/docs_ngweb/source/feature_edit.html#ngw-attachments>`_ and display them in NextGIS Web.

Launch the tool: https://toolbox.nextgis.com/t/panotag

Example:

.. figure:: _static/panotag_input.png
   :name: panotag_input_pic
   :align: center
   :width: 16cm

   Untagged image

.. figure:: _static/panotag_result.png
   :name: panotag_result_pic
   :align: center
   :width: 16cm

   Tags allow the image to be viewed as a spherical panorama

**Try the tool in action by downloading our example:**

`Input data set <https://nextgis.ru/data/toolbox/panotag/panotag_inputs.zip>`_ to test the tool. The archive contains step-by-step instructions.

`Result example <https://nextgis.ru/data/toolbox/panotag/panotag_outputs.zip>`_ of the tool run.
