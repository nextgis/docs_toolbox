Improve DEM
===============

Improves Digital Elevation Model, makes the resulting contour lines smoother and simpler.


Input, all fields are required:


* **Raster file** - DEM file in TIFF format downloaded from NextGIS Data;
* **Interpolation method** used to enhance the DEM file. Available methods: 

  - Nearest neighbor (nearest)
  - Bilinear (bilinear)
  - Cubic (cubic)
  - Cubic spline (cubicspline)
  - Lanczos (lanczos)
  - Linear (average)
  - RMS (rms)
  - Mode (mode);

* **Interval between contours** - Vertical step of the contour lines in meters;
* **Simplification step** for the contour lines. Integer (for example, 2), decimal separated by a dot (for example, 0.02) or exponential notation (for example, 2e-2)
* **Refinement, %** - Improvement of the DEM file resolution, in percents. Shows how much the pixel size should increase/decrease. For example, a value of 1000 % will result in 10 times smaller pixels

Output:

* TIFF file of the refined DEM;
* GeoPackage file of the contour lines.

.. figure:: _static/improvedem_input.png
   :name: improvedem_input_pic
   :align: center
   :width: 10cm

   Input raster

.. figure:: _static/improvedem_result.png
   :name: improvedem_result_pic
   :align: center
   :width: 10cm

   Processed raster and contours generated from it

Launch the tool: https://toolbox.nextgis.com/t/improvedem

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

   * `Polygons topological simplifier <https://toolbox.nextgis.com/t/polysimplifier?from-related-tools=1>`_
   * `Advanced vector generalization <https://toolbox.nextgis.com/t/generalization?from-related-tools=1>`_
   * `Split Complex Polygons <https://toolbox.nextgis.com/t/splitcomplex?from-related-tools=1>`_
