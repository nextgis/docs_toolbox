Split into rectangles and calculate their number
================================================

Splits polygon layer into equal rectangular parts and calculates number of rectangles. Layer can consist of several polygons, number of rectangles will be calculated for each of them. 

Inputs:

*  Shapefile - polygonal layer in ESRI Shapefile format, for which the number of rectangles will be calculated. Should be packed in ZIP-archive. Attributes should contain empty integer field, where the results of calculation will be recorded. Layer CRS must be use meters, EPSG:4326 is not suitable.
* Length of rectangle - longer side of rectangle, should be specified in meters.
* Width of rectangle - shorter side of rectangle, should be specified in meters.
* Field name - name of the string field in initial layer, where to write the number of calculated rectangles for each polygon.
* Percentage of not filled area – please, specify percentage. Percentage is calculated out of rectangle area and will be used to form a buffer around each rectangle.

Outputs:

* ZIP-archive with modified Shapefile, with a number of rectangles recorded in attribute table. 

Launch the tool: https://toolbox.nextgis.com/t/split_to_rect

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

   * `Generate a set of squares with transects <https://toolbox.nextgis.com/t/quadro?from-related-tools=1>`_
   * `Meter grid <https://toolbox.nextgis.com/t/grid?from-related-tools=1>`_