Convert Garden Gnome Package panoramas to JPEG
==============================================

Extracts panoramas from a Garden Gnome Package (.ggpkg) exported by Pano2VR and converts them into flat equirectangular JPEG images, one per shooting point of the tour. The result is a ZIP archive with the panoramas, ready to be uploaded to NextGIS Web.

Inputs:

* Source package. Tour in Garden Gnome Package format (.ggpkg), exported from Pano2VR.

Outputs:

* ZIP archive with equirectangular JPEG panoramas, one per shooting point.

These panoramas can be added as attachments to vector layer features and viewed on a Web Map in NextGIS Web, `learn more <https://docs.nextgis.com/docs_ngweb/source/feature_edit.html#ngw-attachments-panoramas>`_.

Launch the tool: https://toolbox.nextgis.com/t/pano2vr

Example:

.. todo:: _static/pano2vr_input_en.png
   :name: pano2vr_input_pic
   :align: center
   :width: 20cm

   Example input

.. todo:: _static/pano2vr_result_en.png
   :name: pano2vr_result_pic
   :align: center
   :width: 20cm

   Example output


**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.

.. admonition:: Related tools

   * `Add Google Photosphere XMP metadata to photos <https://toolbox.nextgis.com/t/panotag?from-related-tools=1>`_
   * `Photos with EXIF to NGW layer <https://toolbox.nextgis.com/t/exif2resource?from-related-tools=1>`_
   * `Geotag photos using GPX track <https://toolbox.nextgis.com/t/gpx2exif?from-related-tools=1>`_