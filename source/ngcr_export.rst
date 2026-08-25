NextGIS Container Registry image export
=======================================

Export Docker images from NextGIS Container Registry to \*.tar.gz archive. This helps to install or update software on servers in air-gapped environments.

You can run the export tool using any NextGIS ID account, including the free plan, but when running the tool you will need to provide your login and password for access to NextGIS Container Registry.

.. admonition:: Instructions on how to install and update NextGIS server software

   * `NextGIS Web <https://docs.nextgis.com/docs_ngweb/source/ngw_op.html>`_
   * `GeoServices <https://docs.nextgis.com/docs_geoserv_prem/source/index.html>`_
   * `NextGIS Toolbox <https://docs.nextgis.com/docs_toolbox_prem/source/index.html>`_

Inputs:

* Distribution:

  - NextGIS Web Standard
  - NextGIS Web Standard + Whitelabel
  - NextGIS Web Extended
  - NextGIS Web Extended + Whitelabel
  - NextGIS GeoServices
  - NextGIS Toolbox
  - Nominatim
  - BusyBox (test)

* Version. Specify the product version to export Docker images for.
* Login and password for accessing the NextGIS Container Registry. Provided by NextGIS Support with the product delivery.

Outputs:

* \*.tar.gz archive. Images can be imported into Docker using the command ``docker load -i <archive_name>.tar.gz``.

Launch the tool: https://toolbox.nextgis.com/t/ngcr_export

Example:

.. todo:: _static/ngcr_export_input_en.png
   :name: ngcr_export_input_pic
   :align: center
   :width: 20cm

   Example input

.. todo:: _static/ngcr_export_result_en.png
   :name: ngcr_export_result_pic
   :align: center
   :width: 20cm

   Example output


**Try the tool in action**

1. Click on the **Demo** button above the tool form. The fields are filled in with demo values.
2. Click on the **Run** button.
