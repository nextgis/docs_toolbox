Advanced vector generalization
==============================

Simplification of vector layer features to reduce data volume.

Inputs:

* Vector layer. Layer in ESRI Shapefile format, packed in a ZIP archive;
* Merging of nodes. The value (in coordinate system units) at which geometry nodes begin to merge with each other. Default is -1 and corresponds to the absence of merging of nodes. Optional;
* Number of iterations. An integer indicating the number of iterations of the simplification, smoothing, or shifting procedure. Optional;
* Method. Choose a generalization method: ``douglas, douglas_reduction, lang, reduction, reumann, boyle, sliding_averaging, distance_weighting, chaiken, hermite, snakes, displacement``;
* Threshold. Required parameter. If the method does not refer to this parameter, specify any number;
* Number of points. An integer that specifies the number of points used in some methods. Optional. The default value is 7;
* Reduction. A number from 0 to 100. In the simplification algorithm, it characterizes the percentage of points that are preserved relative to the original number of points. An optional parameter. The default value is 50;
* Slide. A number from 0 to 1, characterizes the shift of the obtained point relative to the original. Optional parameter. The default value is 0.5;
* Minimum angle. A number from 0 to 180. Specifies the minimum angle between two consecutive line segments. Optional. The default value is 3;
* Alpha. Number, parameter for the Snakes method. Optional. The default value is 1;
* Beta. Number, parameter for the Snakes method. Optional. The default value is 1.

Output:

* Layer in ESRI Shapefile format, packed in a ZIP archive.



 

The result of the process is a layer with simplified features (geometries).

Launch tool: https://toolbox.nextgis.com/operation/generalization

View the result on an interactive map: https://demo.nextgis.com/resource/4108/display?panel=info

**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/generalization/generalization_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/generalization/generalization_outputs.zip>`_ to additionally check the results.

More on startup options: https://grasswiki.osgeo.org/wiki/V.generalize_tutorial
