Выгрузка из реестра контейнеров NextGIS
=======================================

Выгрузка образов Docker из реестра контейнеров NextGIS в архив *.tar.gz. Это позволяет производить установку и обновление ПО в отсутствие выхода в интернет.

.. admonition:: Инструкции по обновлению серверного ПО NextGIS

   * `GeoServices <https://docs.nextgis.ru/docs_geoserv_prem/source/upgrade.html>`_
   * `NextGIS Web <https://docs.nextgis.ru/docs_ngweb/source/op_upgrade.html>`_
   * `NextGIS Toolbox <https://docs.nextgis.ru/docs_toolbox_prem/source/admin.html#nextgis-toolbox>`_
   * `Nominatim <https://docs.nextgis.ru/docs_howto/source/geocoder_onprem.html>`_

На входе:

* Дистрибутив. Выберите один из вариантов:

  - NextGIS Web Standard (nextgisweb/std)
  - NextGIS Web Standard + Whitelabel (nextgisweb/std-wl)
  - NextGIS Web Extended (nextgisweb/ext)
  - NextGIS Web Extended + Whitelabel (nextgisweb/ext-wl)
  - NextGIS GeoServices (geoservices)
  - NextGIS Toolbox (toolbox,toolbox-tool)
  - Nominatim (nominatim)
  - BusyBox (test) (busybox)

* Версия дистрибутива;
* Логин к реестру контейнеров;
* Пароль к реестру контейнеров.

На выходе:

* Файл TAR.GZ.

Запуск инструмента: https://toolbox.nextgis.com/t/ngcr_export

Пример работы инструмента:

.. todo:: _static/ngcr_export_input_ru.png
   :name: ngcr_export_input_pic
   :align: center
   :width: 20cm

   Пример исходных данных

.. todo:: _static/ngcr_export_result_ru.png
   :name: ngcr_export_result_pic
   :align: center
   :width: 20cm

   Пример результата работы инструмента

**Попробуйте инструмент в действии:**

1. Нажмите кнопку **Демо** над формой инструмента. Поля будут автоматически заполнены демонстрационными значениями.
2. Нажмите кнопку **Запустить**.

