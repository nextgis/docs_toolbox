Count number of layer intersections
==========================================

The tool counts the number of intersections between 2 sets of layers, one of the sets should contain only polygons. In other words, the tool finds, how many objects lay within area of interest, defined by polygons. The result is CSV file with information about each polygon.

Input:

* Area of interest - a set with one or several GeoJSON files, packed in ZIP-archive. Each file should consist only of 1 polygon. Names of the files will be displayed in resulting CSV.
* Objects - one or several vector layers of any geometry type (could differ among layers) in Esri Shapefile or GeoPackage format. Layer or layers should be packed in ZIP-archive.
* Group by layer - optional field. If the box is checked, data in CSV will be grouped by objects' layers. Otherwise - by geometry types of the objects.
* Separate records - optional field. If the box is checked, each category value (layers or geometry types, depending on the choice above) will be put into a separate record.

Output:

* CSV file with information, how many objects and of which geometry type lay within each polygon. 


Launch the tool: https://toolbox.nextgis.com/t/crossing_borders

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

   * `Intersector <https://toolbox.nextgis.com/t/ngw_intersect?from-related-tools=1>`_
   * `Polygon intersection <https://toolbox.nextgis.com/t/vectorclip?from-related-tools=1>`_