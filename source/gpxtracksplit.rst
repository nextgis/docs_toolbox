Разрезать GPX-файл на треки
===========================

Разделяет GPX-файл на отдельные файлы по трекам.

На входе:

* Исходный GPX-файл, который будет разрезаться по трекам. Если у вас много файлов, то сначала склейте их в один инструментом `Объединение треков GPX <https://toolbox.nextgis.com/t/gpxmerge>`_.

На выходе:

* ZIP-архив с отдельными GPX-файлами.

Запуск инструмента: https://toolbox.nextgis.com/t/gpxtracksplit

Пример работы инструмента:

.. todo:: _static/gpxtracksplit_input_ru.png
   :name: gpxtracksplit_input_pic
   :align: center
   :width: 16cm

   Пример исходных данных

.. figure:: _static/gpxtracksplit_result_ru.png
   :name: gpxtracksplit_result_pic
   :align: center
   :width: 20cm

   Пример результата работы инструмента: три отдельных трека

**Попробуйте инструмент в действии, скачав наш пример:**

1. Нажмите кнопку **Демо** над формой инструмента. Поля будут автоматически заполнены демонстрационными значениями.
2. Нажмите кнопку **Запустить**.

.. admonition:: Связанные инструменты

   * `Объединение треков GPX <https://toolbox.nextgis.com/t/gpxmerge>`_
   * `Разбивка GPX-файла по дням <https://toolbox.nextgis.com/t/gpxdailysplit>`_
   * `Обрезка GPX файла по прямоугольнику <https://toolbox.nextgis.com/t/gpxclipbbox>`_
   * `Добавление координат к фотографиям <https://toolbox.nextgis.com/t/gpx2exif>`_