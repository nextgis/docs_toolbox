NextGIS Container Registry export
=================================

Export Docker images from NextGIS Container Registry to *.tar.gz archive. This allows to update or install software on servers with no Internet connection.

You can run the export tool using any NextGIS ID account, including the free plan, but when running the tool you will need to provide your login and password for access to NextGIS Container Registry.

.. admonition:: Instructions on how to update NextGIS software

  * `NextGIS Web <https://docs.nextgis.com/docs_ngweb/source/op_upgrade.html>`_
  * `NextGIS GeoServices <https://docs.nextgis.com/docs_geoserv_prem/source/upgrade.html>`_
  * `NextGIS Toolbox <https://docs.nextgis.com/docs_toolbox_prem/source/admin.html>`_

Inputs:

* Distribution:

  - NextGIS Web Standard (nextgisweb/std)
  - NextGIS Web Standard + Whitelabel (nextgisweb/std-wl)
  - NextGIS Web Extended (nextgisweb/ext)
  - NextGIS Web Extended + Whitelabel (nextgisweb/ext-wl)
  - NextGIS GeoServices (geoservices)
  - NextGIS Toolbox (toolbox,toolbox-tool)
  - Nominatim (nominatim)
  - BusyBox (test) (busybox)

* Version. Specify the product version to export Docker images for. You can check the distribution version used in the ``docker-compose.yaml`` file under ``services.app.image``; for example, the value ``cr.nextgis.com/nextgisweb/std/app:3.3.0`` corresponds to version ``3.3.0``.
* Login and password for accessing the NextGIS Container Registry. Provided by NextGIS Support with the product delivery.


Outputs:

* TAR.GZ file.

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
