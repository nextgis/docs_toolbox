Координаты центра в атрибуты
============================

Инструмент рассчитывает центр полигона (PointOnSurface), добавляет поля point_X, point_Y с координатами точки, гарантировано находящейся внутри полигона. Работает только с полигонами.

На входе:

* Полигональный слой - векторный слой в одном из поддерживаемых GDAL форматов, например, Shapefile в ZIP-архиве, GeoJSON, GeoPackage.

На выходе:

* ZIP-архив с shp-файлом слоя полигонов, содержащим два новых поля point_X, point_Y 
* Файл стиля .qml

.. figure:: _static/point_on_surface.png
   :align: center
   :width: 16cm

   
.. figure:: _static/point_on_surface_attributes.png
   :align: center
   :width: 16cm
   

Запуск инструмента: https://toolbox.nextgis.com/operation/centroid2attr

**Попробуйте инструмент в действии, скачав наш пример:**

`Набор исходных данных <https://nextgis.ru/data/toolbox/centroid2attr/centroid2attr_inputs.zip>`_ для проверки работы инструмента. Внутри архива пошаговая инструкция.

`Пример результата <https://nextgis.ru/data/toolbox/centroid2attr/centroid2attr_outputs.zip>`_ работы инструмента.

