Copernicus Sentinel image search
===================================


The tool generates a list of Sentinel scenes in the Copernicus archive that match the specified parameters.

Inputs:

* Image search area - vector file in single-file OGR compatible fomats with SRS (Recomended: GeoJSON EPSG:4326). The file must contain exactly one feature. Avaliable geometry types: Point, LineString, Polygon. We recommend to use geometries with a small number of vertices.
* Start date of the sensing period in UTC format (images from this date are **included** in the result). By default the first day of the current month is used.
* End date of the sensing period in UTC format (images from this date are **not included** in the result). By default the current date is used.
* Mission - choose mission (collection):

  - Sentinel-2 (Sentinel-2)
  - Sentinel-1 (Sentinel-1)
  - Sentinel-3 (Sentinel-3)

* Products. By default searches all products, but you can specify one of the following:

  - for Sentinel-2: ``S2MSI1C, S2MSI2A``;
  - for Sentinel-1:  ``RAW, SLC, GRD, OCN``;
  - for Sentinel-3: ``OL_1_EFR___, OL_1_ERR___, OL_2_LFR___, OL_2_LRR___, OL_2_WFR___, OL_2_WRR___, SL_1_RBT___, SL_2_AOD___, SL_2_FRP___, SL_2_LST___, SL_2_WST___, SR_1_SRA___, SR_1_SRA_A_, SR_2_LAN___, SR_2_WAT___, SY_2_AOD___, SY_2_SYN___, SY_2_V10___, SY_2_VG1___, SY_2_VGP___``

* Sensor mode. For Sentinel-2 or Sentinel-3 leave this field empty. For Sentinel-1, the default is all modes, or you can choose:

  - Stripmap (SM)
  - Interferometric Wide Swath (IW)
  - Extra Wide Swath (EW)
  - Wave (WV)

* Cloud cover (maximum) - Only for Sentinel-2. Maximal cloud cover in percentage. If field value is epmty, apply default value - 100%.

Outputs:

* XLSX file containing a list of scene IDs.
* Text report containing the total number of scenes and the IDs of the first ten scenes.

Launch the tool: https://toolbox.nextgis.com/t/imagesearch

**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

  * `Search and save Sentinel-2 scene previews <https://toolbox.nextgis.com/t/s2_search?from-related-tools=1>`_
  * `Prepare and download Sentinel-2 data <https://toolbox.nextgis.com/t/download_and_prepare_l8_s2?from-related-tools=1>`_
  * `Image clustering <https://toolbox.nextgis.com/t/image_clustering?from-related-tools=1>`_
  * `Image classification <https://toolbox.nextgis.com/t/image_classification?from-related-tools=1>`_
