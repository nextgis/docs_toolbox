Растр с AUX XML ESRI в GeoTIFF
============================================

Исправляет проблему с геопривязкой в растре в формате JPG с AUX XML ESRI. По умолчанию, такие растры могут неправильно отображаться в QGIS и другом GDAL-зависимом ПО.

На входе:

* Исходный растр - GDAL-совместимый растр с AUX XML в ZIP файле.
* Система координат - Опционально. Описание системы координат в виде строки proj. Если не указана - СК берется из AUX XML.

На выходе:

* Файл GeoTIFF.

Запуск инструмента: https://toolbox.nextgis.com/t/esriauxxml2geotiff

.. seealso::

   * `Конвертация MapInfo для QGIS <https://toolbox.nextgis.com/t/mapinfo2qgis?from-related-tools=1>`_
   * `Конвертация векторных слоев <https://toolbox.nextgis.com/t/convert?from-related-tools=1>`_

