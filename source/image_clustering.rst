Image clustering 
=================


Performs automatic clustering of an image (e.g. satellite image) into a specified number of classes. K-Means algorithm is used

Input: 

* Image in GDAL-compatible format (preferably GeoTIFF). It can contain any number of bands, all of which will be used for cluster calculation.

Parameters that can be set up:

* Number of clusters into which the original image will be divided.

* Method of K-Means initialization. Select 'k-means++' or 'random'. ‘k-means++’ selects initial cluster centroids so as to make them furhter apart. This technique speeds up convergence.

* Maximum number of iterations of the k-means algorithm for a single run. Leave empty to use default value (300).

The necessary number of iterations depends on many factors including centroid characteristics and number of clusters. Usually between several dozens and several hundreds iterations are enough.

* K-means algorithm to use. Select 'lloyd' or 'elkan'.

Lloyd's algorithm is the classical EM-style algorithm. The "elkan" variation can be more efficient on some datasets with well-defined clusters, by using the triangle inequality. However it’s more memory intensive.



Output: 

* Clustered image.

.. raw:: html

   <iframe width="560" height="315" src="https://www.youtube.com/embed/Ib9bwQPGLro?si=Y3X6CRytMrpcCYiL" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Watch the video on `youtube <https://youtu.be/Ib9bwQPGLro>`_.

Launch the tool: https://toolbox.nextgis.com/t/image_clustering


**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

  * `Image classification <https://toolbox.nextgis.com/t/image_classification?from-related-tools=1>`_
  * `Normalized difference index <https://toolbox.nextgis.com/t/ndi?from-related-tools=1>`_
  * `Search and save Sentinel-2 scene previews <https://toolbox.nextgis.com/t/s2_search?from-related-tools=1>`_
  * `Prepare and download Sentinel-2 data <https://toolbox.nextgis.com/t/download_and_prepare_l8_s2?from-related-tools=1>`_
