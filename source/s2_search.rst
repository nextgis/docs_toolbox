Sentinel-2 scenes to GPKG 
============================

Search and save Sentinel-2 scene previews to GPKG.

Input:

* **S2 tile index(es)** - Simple or list e.g. "36VWJ" or "36VWJ,36VXJ" - limit 50 id. You can check the ID of the scene you need on our `Web Map <https://demo.nextgis.com/resource/7697/display?panel=layers>`_ or  :download:`download the scene division file <files/sentinel_2_index.gpkg>`;
* **Year(s)** - Simple,list or range e.g. "2016,2020,2021-2024";
* **Month(s)** - Simple,list or range e.g. "1,5,9-12";
* **Max cloud** - Max cloud coverage in %, int or float e.g. 10 or 10.5;
* **Custom order name** - optional, you can enter a name for the Toolbox task to make it easier to tell them apart without comparing all the parameters.

There is also **No preview** option. If ticked, the resulting GeoPackage will contain only vector footprint itendifiers.


Output:

* GPKG file.

If previews are included, to view the result in QGIS select Project ‣ Open From ‣ GeoPackage.

Project also includes a layer with geometries of selected S2 tiles and a search_result layer containing scene IDs, attributes and borders of satellite images from dataspace catalog.

By default, tile layer and the earliest preview are visible. Select the layers you want to display.

.. figure:: _static/s2_search_output_en.png
   :name: s2_search_output_pic
   :align: center
   :width: 20cm

   Search result with layer visibility enabled

Launch instrument: https://toolbox.nextgis.com/t/s2_search

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

   * `Prepare and download Sentinel-2 data <https://toolbox.nextgis.com/t/download_and_prepare_l8_s2?from-related-tools=1>`_
   * `Copernicus Sentinel image search <https://toolbox.nextgis.com/t/imagesearch?from-related-tools=1>`_
   * `Normalized difference index <https://toolbox.nextgis.com/t/ndi?from-related-tools=1>`_
   * `Image clustering <https://toolbox.nextgis.com/t/image_clustering?from-related-tools=1>`_