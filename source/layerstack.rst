Form multi-channel raster from individual channels
====================================================

Converts an archive with raster channels to a single multi-channel raster composed of selected channels.

Inputs:

* ZIP-archive with single-channel rasters, without subfolders.
* List of channels, comma-separated, e.g. 4,3,2 (number of the source raster, in alphabetical order).

Outputs:

* Multi-channel raster as a TIF file.

Launch the tool: https://toolbox.nextgis.com/t/layerstack

Example:

.. figure:: _static/layerstack_input_en.png
   :name: layerstack_input_pic
   :align: center
   :width: 20cm

   Example input: multiple single-channel rasters

.. figure:: _static/layerstack_result_en.png
   :name: layerstack_result_pic
   :align: center
   :width: 20cm

   Example output: combined RGB raster


**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.


.. admonition:: Related tools

   * `Generate tileset from raster <https://toolbox.nextgis.com/t/raster2tiles?from-related-tools=1>`_
   * `Search & download Planetary Computer <https://toolbox.nextgis.com/t/planetary_search?from-related-tools=1>`_
   * `Raster calculator (GRASS) <https://toolbox.nextgis.com/t/r_mapcalc?from-related-tools=1>`_