Проекция Dae (Collada) в Shapefile
==================================

Получение проекции трехмерных объектов на земную плоскость.

На входе:

* ZIP-архив с DAE и KMZ.  Файлы \*.kmz должны содержать геопривязку моделей \*.dae (координаты полигонов в EPSG:4326, единицы измерения - метрические).

На выходе:

*  Файл GeoJSON

На вход можно подать несколько моделей, на выходе по каждой из них получить отдельный полигон.

Запуск инструмента: https://toolbox.nextgis.com/t/kmldae2footprints

**Попробуйте инструмент в действии, скачав наш пример:**

`Набор исходных данных <https://nextgis.ru/data/toolbox/kmldae2footprints/kmldae2footprints_inputs_ru.zip>`_ для проверки работы инструмента. Внутри архива пошаговая инструкция.

`Пример результата <https://nextgis.ru/data/toolbox/kmldae2footprints/kmldae2footprints_outputs_ru.zip>`_ работы инструмента.

.. seealso::

    * `Обрезать PBF по прямоугольнику <https://toolbox.nextgis.com/t/osmclip_bbox?from-related-tools=1>`_
    * `Конвертация облака точек в тайлсет <https://toolbox.nextgis.com/t/pointcloud2tileset?from-related-tools=1>`_