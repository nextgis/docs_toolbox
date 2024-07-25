Erase from target
=================

A tool that allows you to erase areas from the target layer. Areas to be erased are taken from another layer.

Inputs:

* Vector layer from which some areas are needed to be erased

ZIP archive with ESRI Shapefile or an other file format supported by OGR.

* Vector layer containing features representing areas needed to be erased from the target layer

ZIP archive with ESRI Shapefile or other file format supported by OGR.

The result of the tool’s usage is a new vector layer.

The initial vector layers must have the same coordinate system.

Launch tool: https://toolbox.nextgis.com/operation/eraser

View the source data and the results of calculations on an interactive map: https://demo.nextgis.com/resource/4611/display?panel=info

**Try it out using our sample:**

Download `input dataset <https://nextgis.ru/data/toolbox/eraser/eraser_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.ru/data/toolbox/eraser/eraser_outputs.zip>`_ to additionally check the results.
.. figure:: _static/eraser.png
   :align: center
   :width: 16cm

   An example of the result of the tool’s usage
