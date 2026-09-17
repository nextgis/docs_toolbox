Point Cloud to COPC
===================

Converts point clouds files to Cloud Optimized Point Cloud (COPC).

COPC stores point data organized in a clustered octree. It reduces data transfer time, improves performance, and makes it easier to work with large datasets on cloud platforms. 


Inputs:

* Input point cloud file in any PDAL-supported format (LAS, LAZ, PLY, PCD, PTS, PTX, BPF);
* Source CRS - Set if missing from input file metadata. EPSG code, for example, ``EPSG:4326``;
* Output CRS. Set to reproject the result. EPSG code, for example, ``EPSG:4326``;
* Coordinate precision - for example. ``0.01``. Leave empty to use auto mode;
* Attributes:

  - All (all) - use all attributes;
  - Standard (standard) - use standard COPC attributes subset.

Outputs:

* Cloud Optimized Point Cloud in LAZ format.

Launch the tool: https://toolbox.nextgis.com/t/point_cloud_to_copc

Example:

.. figure:: _static/point_cloud_to_copc.jpg
   :name: point_cloud_to_copc_input_pic
   :align: center
   :width: 16cm

   Point cloud


**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

   * `Convert point cloud into tileset <https://toolbox.nextgis.com/t/pointcloud2tileset?from-related-tools=1>`_