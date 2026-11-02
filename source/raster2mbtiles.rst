Растр в MBTiles
===============

Генерация набора тайлов в формате MBTiles из исходного набора растровых данных (поддерживаемого GDAL).

На входе:

* Исходный растр - GDAL-совместимый растр: RGB, RGBA, одноканальный серый или одноканальный с палитрой;
* Масштабные уровни - Необязательно. Диапазон, например, ``8-14``;
* Имя выходного файла - Необязательно. Имя для выходного файла MBTiles. Расширение *.mbtiles* будет добавлено автоматически.

На выходе:

* Тайлы в формате MBTiles.

Запуск инструмента: https://toolbox.nextgis.com/t/raster2mbtiles

Пример работы инструмента:

.. figure:: _static/raster2mbtiles_input_ru.png
   :name: raster2mbtiles_input_pic
   :align: center
   :width: 20cm

   Исходный растр в NextGIS QGIS

.. figure:: _static/raster2mbtiles_result_ru.png
   :name: raster2mbtiles_result_pic
   :align: center
   :width: 8cm

   Тайлы MBTiles в NextGIS Mobile

**Попробуйте инструмент в действии:**

1. Нажмите кнопку **Демо** над формой инструмента. Поля будут автоматически заполнены демонстрационными значениями.
2. Нажмите кнопку **Запустить**.

.. seealso::

   * `Генерация растровых тайлов из проекта QGIS <https://toolbox.nextgis.com/t/qgis_rastertiles?from-related-tools=1>`_
   * `Генерация векторных тайлов из проекта QGIS <https://toolbox.nextgis.com/t/qgis_vectortiles?from-related-tools=1>`_
   * `Конвертация облака точек в тайлсет <https://toolbox.nextgis.com/t/pointcloud2tileset?from-related-tools=1>`_
   * `Геоданные в PMTiles <https://toolbox.nextgis.com/t/geodata2pmtiles?from-related-tools=1>`_