Вычисление спектральных индексов
================================

Вычисление нормализованных разностных спектральных индексов (NDVI, NDWI, NBR) из временных рядов Sentinel-2 или Landsat. Создает временные агрегаты (среднее, макс., мин., стд. откл., диапазон), выровненные по сетке анализа рельефа.

На входе:

* Пакет спутниковых данных - ZIP-файл из `Скачивание данных Planetary Computer <https://toolbox.nextgis.com/t/planetary_search>`_, содержащий GeoTIFF-файлы каналов Sentinel-2 или Landsat и manifest.json с time_series;
* Спектральный индекс. Тип нормализованного разностного индекса:

  - NDVI (Растительность) (NDVI);
  - NDWI (Вода) (NDWI);
  - NBR (Индекс гарей) (NBR).

На выходе:

* ZIP-архив с агрегатами спектральных индексов, статистикой и манифестом;
* Текстовая сводка результатов спектральных индексов;
* JSON-манифест, описывающий все результаты.

Запуск инструмента: https://toolbox.nextgis.com/t/spectral_indices

Пример работы инструмента:

.. todo:: _static/spectral_indices_input_ru.png
   :name: spectral_indices_input_pic
   :align: center
   :width: 16cm

   Пример исходных данных

.. todo:: _static/spectral_indices_result_ru.png
   :name: spectral_indices_result_pic
   :align: center
   :width: 16cm

   Пример результата работы инструмента

**Попробуйте инструмент в действии:**

1. Нажмите кнопку **Демо** над формой инструмента. Поля будут автоматически заполнены демонстрационными значениями.
2. Нажмите кнопку **Запустить**.

.. seealso::

   * `Нормализованный разностный индекс <https://toolbox.nextgis.com/t/ndi?from-related-tools=1>`_
   * `Калькулятор растров (GDAL) <https://toolbox.nextgis.com/t/raster_calculator?from-related-tools=1>`_
   * `Калькулятор растров (GRASS) <https://toolbox.nextgis.com/t/r_mapcalc?from-related-tools=1>`_