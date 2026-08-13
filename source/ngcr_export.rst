NextGIS Container Registry export
=================================

Export Docker images from NextGIS Container Registry to *.tar.gz archive. This allows to update or install software on servers with no Internet connection.

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

* Version - Distribution version;
* Login for Container Registry;
* Password for Container Registry.

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
