Polygon to explication (forestry)
=================================

Generating a report of explication of forest plots. Used to automatically obtain a table of lengths and azimuths from a polygon.

Inputs:

* Polygonal layer (forest plot) - a vector data set (plot boundaries) in the format supported by OGR. Shape-files are transferred in an archive, single-file sets - uncompressed. There should be only 1 feature on the layer;
* Line layer (reference) - Vector data set (reference) in the format supported by OGR. Shape-files are transferred in an archive, single-file sets - uncompressed. There should be only 1 feature on the layer. If the reference section can not be filled out, the “Stub” can be used instead, which is a layer without features. A stub can be taken :download:`here <files/empty_layer.geojson>`;
* Type on angles to calculate. 

    - Directional angles (0)
    - Magnit azimuth (1)
    - True north azimuth (2)

Magnetic and true angles can be calculated only if the source data (plot polygon and reference line) have correct CRS description. To calculate true angles the data is reprojected to the corresponding UTM zone. To calculate magnetic angles World Magnetic Model is used to calculate deviation;

* Description of the binding method - free text;
* Forestry number - integer.

Outputs:

*  Excel report (XLSX).

Launch the tool: https://toolbox.nextgis.com/t/poly2explication


   
**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/poly2explication/poly2explication_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/poly2explication/poly2explication_outputs.zip>`_ to additionally check the results.
