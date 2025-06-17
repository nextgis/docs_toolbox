Разделить сложные полигоны
==========================

Разделяет полигоны с большим количеством вершин на более мелкие части. Каждая часть представляет собой отдельный объект, сохраняющий все атрибуты исходного полигона.

На входе:

* Исходный файл - векторный слой в одном из поддерживаемых GDAL форматов, например, GeoPackage, Shapefile в ZIP-архиве, GeoJSON.
* Максимальное число вершин - максимально допустимое число вершин в полигоне. По умолчанию — 200000

На выходе:

* Файл GeoPackage с полигонами, разделёнными при превышении порога по числу вершин.


Запуск инструмента: https://toolbox.nextgis.com/t/splitcomplex

.. figure:: _static/splitcomplex_input_ru.png
   :name: splitcomplex_input_pic
   :align: center
   :width: 16cm

   Пример исходных данных

.. figure:: _static/splitcomplex_result_ru.png
   :name: splitcomplex_result_pic
   :align: center
   :width: 16cm

   Пример результата работы инструмента, полигон разбит на составные части

**Попробуйте инструмент в действии, скачав наш пример:**

`Набор исходных данных <https://nextgis.ru/data/toolbox/splitcomplex/splitcomplex_inputs_ru.zip>`_ для проверки работы инструмента. Внутри архива пошаговая инструкция.

`Пример результата <https://nextgis.ru/data/toolbox/splitcomplex/splitcomplex_outputs_ru.zip>`_ работы инструмента.
