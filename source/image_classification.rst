.. sectionauthor:: Юлия Григоренко <grigorenko.j@gmail.com>

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

Launch instrument: https://toolbox.nextgis.com/operation/image_classification

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/ai2geo/image_classification_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/ai2geo/image_classification_outputs.zip>`_ to additionally check the results.
