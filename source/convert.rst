Конвертация векторных слоёв
===========================

Конвертация векторных слоёв между разными форматами файлов.


На входе:

*  Векторный слой. Одиночный файл GeoJSON, GPKG, GPX, KMZ или ZIP-архив с одним векторным слоём любого формата поддерживаемого библиотекой GDAL, например архив с ESRI Shapefile.
*  Название выходного формата.

.. note::
   Если загрузить в инструмент файл неподходящего формата (например, SQL или одиночный файл SHP), появится сообщение об ошибке.

На выходе:

* ZIP архив с векторным слоем. 

Система координат не изменяется. 

Если конвертация в ESRI Shapefile, то атрибуты конвертируются в UTF-8. У остальных форматов кодировка не изменяется, подразумевается что их создатели уже создают их в UTF-8.

Запуск инструмента: https://toolbox.nextgis.com/t/convert

**Попробуйте инструмент в действии, скачав наш пример:**

`Набор исходных данных <https://nextgis.ru/data/toolbox/convert/convert_inputs_ru.zip>`_ для проверки работы инструмента. Внутри архива пошаговая инструкция.

`Пример результата <https://nextgis.ru/data/toolbox/convert/convert_outputs_ru.zip>`_ работы инструмента.

   
.. seealso::

   * `Перепроецирование координат <https://toolbox.nextgis.com/t/coord_recalc?from-related-tools=1>`_
   * `Проверка геометрии <https://toolbox.nextgis.com/t/check_geometries?from-related-tools=1>`_
   * `KML в геоданные <https://toolbox.nextgis.com/t/kml2geodata?from-related-tools=1>`_
   * `Конвертация MapInfo для QGIS <https://toolbox.nextgis.com/t/mapinfo2qgis?from-related-tools=1>`_