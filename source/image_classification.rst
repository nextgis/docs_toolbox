

Image classification 
=====================

Performs automatic classification of an image (e.g. satellite image) based on a vector layer with training polygons. Random Forest algorithm is used.

You'll need to input two files:

* Image in GDAL-compatible format (preferably GeoTIFF). It can contain any number of bands, all of which will be used for classification.

* Polygon vector layer with training objects. Any OGR-compatible vector format (preferably GeoPackage) is supported. Each polygon should have a field with object class number in its attributes.

Set up the parameters:

* Name of the attribute that describes the class number for each object in the training polygons layer. The attribute must be an integer.

* The number of trees in the decision forest. Leave blank to use the default value (100).

* Maximum tree depth. Leave blank to not limit the tree depth.

Output:

* Classified raster.
* Classification report. It records the overall quality of the classification, the number of misclassified pixels in each class (and indicates the classes to which they were put instead).

.. raw:: html

   <iframe width="560" height="315" src="https://www.youtube.com/embed/S7APVbtR-5s?si=iEuQf3VO8YUPx0PW" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Watch the video on `youtube <https://youtu.be/S7APVbtR-5s>`_.

Launch instrument: https://toolbox.nextgis.com/t/image_classification

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

   * `Image clustering <https://toolbox.nextgis.com/t/image_clustering?from-related-tools=1>`_
   * `Normalized difference index <https://toolbox.nextgis.com/t/ndi?from-related-tools=1>`_
   * `Search and save Sentinel-2 scene previews <https://toolbox.nextgis.com/t/s2_search?from-related-tools=1>`_
   * `Prepare and download Sentinel-2 data <https://toolbox.nextgis.com/t/download_and_prepare_l8_s2?from-related-tools=1>`_