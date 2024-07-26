Image clustering 
=================


Performs automatic clustering of an image (e.g. satellite image) into a specified number of classes. K-Means algorithm is used

Parameters that can be set up:

* Number of clusters into which the original image will be divided.
* Method of K-Means initialization. Could be 'k-means++' or 'random'. Leave empty to use default value (k-means++).
* Maximum number of iterations of the k-means algorithm for a single run. Leave empty to use default value (300).
* K-means algorithm to use. Could be one of 'lloyd', 'elkan'. Leave empty to use default value (lloyd)

Input: Image in GDAL-compatible format (preferably GeoTIFF). It can contain any number of bands, all of which will be used for cluster calculation.

Output: Clustered image.

Launch tool: https://toolbox.nextgis.com/operation/image_clustering


**Try it out using our sample:**

Download `input dataset <https://nextgis.com/data/toolbox/xml_decl_to_vector/xml_decl_to_vector_inputs.zip>`_ to test the instrument. Step-by-step instructions included.

Get the `output <https://nextgis.com/data/toolbox/xml_decl_to_vector/xml_decl_to_vector_outputs.zip>`_ to additionally check the results.
